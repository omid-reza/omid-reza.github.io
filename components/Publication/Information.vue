<template>
	<div>
		<div class="alert alert-warning">
			<div class="mb-0">
				<span v-for="(author, index) in pub.authors">
					<span v-if="index == Object.keys(pub.authors).length - 1">and</span>
					{{ author }}
					<span v-if="index != Object.keys(pub.authors).length - 1">; </span>
				</span>
				<br>
				<b>{{ pub.title }}</b>
				<br>
				<span v-for="(destination, text, index) in pub.links">
					<a :href="destination" class="text-decoration-none">
						{{text}}
					</a>
					<span v-if="index != Object.keys(pub.links).length - 1">|</span>
				</span>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	props:['pub']
}
</script>