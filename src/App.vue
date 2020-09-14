<template>
	<div id="nav">
		<AppHeader />
	</div>
	<router-view />
</template>
<script>
	import AppHeader from "@/components/global/AppHeader.vue";
	export default {
		name: "app",
		components: { AppHeader },
	};
</script>








<style lang="scss">
	#app {
		font-family: Avenir, Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
	}
</style>
