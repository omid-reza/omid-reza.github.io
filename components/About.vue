<template>
	<div id="about">
		<div class="alert alert-success">
			<h3 class="alert-heading">
				About Me
			</h3>
			<p class="mb-0" v-html="text"></p>
		</div>
	</div>
</template>

<script>
export default {
	data(){
		return{
			'text':'I completed my B.Sc. in Computer Science from Islamic Azad University. Moreover, I am avid about working with data. Hence, I have commenced working in data-related areas, namely Artificial intelligence and Signal Processing. Added to the prior, I operated as a Back-end developer for a few years before switching to the current fields.'
		}
	}
}
</script>