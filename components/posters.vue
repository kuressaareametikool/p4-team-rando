<template>
	<ul>
		<li v-for="(post,index) of posts" :key="index">{{ post.title }}</li>	
	</ul>
</template>
<script>
export default {
   async asyncData({ $content }) {
    const posts = await this.$content("Poster").fetch();

    return {
      posts,
    };
  },
};
</script>