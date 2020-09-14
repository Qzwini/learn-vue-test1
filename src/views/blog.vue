<template>
	<div class="blog">
		<div class="container">
			<h1>{{ pageName }}</h1>
			<p> {{ pageDescription }} </p>

			<div class="row">
				<div class="col-md-8">
					<div class="posts-area">
						<BlogPost
							v-for="post in posts"
							:key="post.id"
							:views="post.views"
							:title="post.title"
							:date="post.date"
							:content="post.content"
							:auther="post.auther"
							:category="post.category"
						/>
					</div>
				</div>

				<div class="col-md-4">
					<div class="sidebar">
						<blogSidebar />

					</div>
				</div>
			</div>

			<but />

		</div>
	</div>
</template>

<script>
	import BlogPost from "@/components/blog/blogPosts.vue";
	import blogSidebar from "@/components/blog/blogSidebar.vue";
	import but from "@/components/blog/but.vue";
	import jsonPost from "../json/postData.json";

	export default {
		data: function () {
			return {
				pageName: "blog",
				pageDescription: "This is blog Page",
				posts: jsonPost,
			};
		},
		name: "blog",
		components: {
			BlogPost,
			blogSidebar,
			but,
		},
	};
</script>






