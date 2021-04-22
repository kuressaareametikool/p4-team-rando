<template>
	<div>
		<img v-for="(poster,index) in posters" :key="index" :src="poster.poster" alt="">
	</div>
</template>
<script>
export default {
	props: {
		posters: {
			type: Array,
			default: []
		}
	}
};
</script>