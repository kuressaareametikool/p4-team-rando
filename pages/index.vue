<template>
  <div class="poster">
      <logo class="absolute left-0 ml-12" />
    <div class="info">
      <info />
    </div>
    <div class="picture">
      <posters :posters="posters" />
    </div>
  </div>
</template>

<script>
import logo from "../components/Logo";
import contacts from "../components/contacts";
import posters from "../components/posters";
import info from "../components/info";
export default {
  async asyncData({ $content }) {
    const posters = await $content("Poster").fetch();

    return {
      posters,
    };
  },
  head() {
    return {
      link: [
        { rel: 'stylesheet', href: "https://fonts.googleapis.com/css2?family=Playfair+Display&display=swap" }, 
        { rel: 'stylesheet', href: "https://fonts.googleapis.com/css2?family=Oswald:wght@200&family=Playfair+Display&display=swap" }
      ],
        script: [{ src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }],
    };
  },
  components:{
    contacts, posters, info, logo
  },
  created(){
    window.setInterval(() => {
      const date = new Date();

      if(date.getHours() === 3 && date.getMinutes() === 0 && date.getSeconds() === 0) {
        window.location.reload();
      }
    }, 1000);
  }
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
