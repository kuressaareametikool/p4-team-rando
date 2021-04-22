<template>
	<div class="h-full">
        <hooper :autoPlay="true" :playSpeed="2000" style="height: 100%">
            <slide v-for="(poster,index) in posters" :key="index">
                <img  :src="poster.poster" alt="" class="h-full w-full ">
            </slide>
        </hooper>
    </div>
</template>
<script>
import { Hooper, Slide } from 'hooper';
import 'hooper/dist/hooper.css';
export default {
	props: {
		posters: {
			type: Array,
			default: []
		}
	},
    components: {
        Hooper,Slide
  }
};
</script>
