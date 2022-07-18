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
			'text':'I completed my B.Sc. in Computer Science from Islamic Azad University. Moreover, I am avid about working with data. Ergo, I have started to work in the "Machine learning" and "Signal processing" fields. In addition, I used to operate as a Back-end developer for a few years.'
		}
	}
}
</script>