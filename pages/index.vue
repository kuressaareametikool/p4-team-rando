<template>
  <div class="poster">
      <logo class="absolute left-0 ml-12" />
    <div class="info"></div>
    <div class="picture">
      <posters :posters="posters" />
    </div>
  </div>
</template>

<script>
import logo from "../components/Logo";
import contacts from "../components/contacts";
import posters from "../components/posters";
export default {
  async asyncData({ $content }) {
    const posters = await $content("Poster").fetch();

    return {
      posters,
    };
  },
    head() {
    return {
        script: [{ src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }],
    };
    components:{
      contacts, posters, logo
    }
  },
};
</script>

<style>
.poster {
  display: flex;
  justify-content: center;
  position: absolute;
  top: 50%;
  left: 50%;
  margin-right: -50%;
  transform: translate(-50%, -50%);
  width: 1080px;
  height: 1920px;
  background-color: #40362d;
}

.picture {
  margin-right: auto;
  margin-left: auto;
  margin-top: 100px;
  width: 841px;
  height: 1189px;
  background-color: white;
}

.info {
  position: absolute;
  bottom: 0px;
  width: 1080px;
  height: 470px;
  background-color: #2a221b;
}
</style>
