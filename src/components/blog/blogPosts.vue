<template>
	<div class="post-box">
		<span class="post-views">{{views}}</span>
		<h3 class="post-title">{{title}}</h3>
		<span class="post-date">{{date}}</span>
		<p class="post-content">
			{{content}}
		</p>
		<div class="row">
			<div class="col-sm-6">
				<spam class="post-au">{{auther}}</spam>
			</div>
			<div class="col-sm-6 text-right">
				<spam class="post-cat">{{category}}</spam>
			</div>

		</div>
	</div>

</template>

<script>
	export default {
		props: ["views", "title", "date", "content", "auther", "category"],
		name: "post",
	};
</script>


<style lang="scss">
	$size: 30px;
	$bg: #d4edda;
	.post-box {
		background-color: #fff;
		padding: 20px;
		box-shadow: 0 0 10px #ddd;
		border-radius: 5px;
		position: relative;
		text-align: left;
		margin: 10px 0;
		.post-views {
			position: absolute;
			color: #607d8b;
			top: 5px;
			right: 5px;
			background-color: #d4edda;
			border-radius: 5px;
			padding: 5px;
			text-align: center;
			width: $size * 2;
			height: $size;
			font-weight: bold;
		}
		.post-title {
			font-weight: bold;
			color: #818080;
		}
		.post-date {
			display: block;
			padding: 0 0 5px;
			color: #888;
			font-size: 14px;
		}

		.post-au,
		.post-cat {
			// display: block;
			background-color: #607d8b;
			padding: 6px 10px;
			border-radius: 5px;
			color: #fff;
			// margin:auto;
			// text-align: center;
		}
	}
</style>