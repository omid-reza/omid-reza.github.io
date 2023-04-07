<template>
	<div>
		<div :class="cls">
			<div class="mb-0">
				<span v-for="(author, index) in pub.authors">
					<span v-if="index == Object.keys(pub.authors).length - 1">and</span>
					{{ author }}
					<span v-if="index != Object.keys(pub.authors).length - 1">; </span>
				</span>
				<br>
				<b>{{ pub.title }}</b>
				<br>
				<span v-for="(link, index) in pub.links">
					<a :href="link.destination" class="text-decoration-none">
						<img :src="link.image" class="ico icon" />
					</a>
					{{ link.text }}
					<span v-if="index != Object.keys(pub.links).length - 1">|</span>
				</span>
			</div>
		</div>
	</div>
</template>

<style>
.icon{
	width: 70px;
	height: 70px;
}	
</style>

<script>
export default {
	props:['pub', 'cls']
}
</script>