<template>
	<div class="but">
		<div
			class="alert alert-success alert-dismissible fate show"
			role="alert"
		>
			Learn vue
			<button
				type="button"
				class="close"
				data-dismiss="alert"
				aria-label="Close"
			>
				<span aria-hidden="true">&times;</span>
			</button>
		</div>
	</div>
</template>

<script>
	export default {
		name: "but",
	};
</script>

<style lang="scss">
	.but{
		margin: 15px 0;
	
	}
</style>