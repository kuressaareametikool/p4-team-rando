<template>
  <div class="h-full">
    <hooper :autoPlay="true" :playSpeed="2000" style="height: 100%">
      <slide v-for="(poster, index) in posters" :key="index">
        <img :src="poster.poster" alt="" class="h-full w-full" />
      </slide>
      <hooper-pagination slot="hooper-addons"></hooper-pagination>
    </hooper>
  </div>
</template>
<script>
import { Hooper, Slide, Pagination as HooperPagination } from "hooper";
import "hooper/dist/hooper.css";
export default {
  props: {
    posters: {
      type: Array,
      default: [],
    },
  },
  components: {
    Hooper,
    Slide,
    HooperPagination,
  },
};
</script>
<style scoped>
.hooper-pagination {
  position: absolute;
  bottom: -50px;
  right: 50%;
  transform: translateX(50%);
  display: flex;
  padding: 5px 10px;
}
</style>
