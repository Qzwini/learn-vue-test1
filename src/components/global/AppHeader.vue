<template>
	<div class="header">
		<div class="container">
			<div class="logo">qzwini Vue</div>
			<ul class="text-right">
				<li>
					<router-link
						to="/"
						exact
					>
						<a>Home</a>
					</router-link>
				</li>

				<li>
					<router-link
						to="/blog"
						replace
					>
						<a>Blog</a>
					</router-link>
				</li>

				<li>
					<router-link to="/about">
						<a>About</a>
					</router-link>
				</li>

				<li>
					<router-link
						to="/help"
						replace
					>
						<a>Help</a>
					</router-link>
				</li>
			</ul>
		</div>
	</div>
</template>

<script>
	export default {
		name: "AppHeader",
	};
</script>


<style lang="scss">
	$bgCol: #333;
	$col: #fff;

	.header {
		background-color: $bgCol;
		color: $col;
		overflow: hidden;
		margin-bottom: 20px;
		.logo {
			font-size: 24px;
			padding: 20px;
			float: left;
			width: 200px;
		}
		.text-right {
			float: right;
		}
		ul {
			width: calc(100%-200px);
			margin: 0;
			padding-right: 20px;

			li {
				display: inline-block;
				font-size: 18px;
				margin: 25px;

				a {
					color: $col;
					text-decoration: none;
				}
			}
		}
	}
</style>