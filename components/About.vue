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
			'text':'I completed my B.Sc. in Computer Science from Islamic Azad University. Moreover, I am avid about working with data. Additionally, I have worked in the "Machine learning" and "Signal processing" fields. What\'s more, I am working on EEG(electroencephalogram) data. Furthermore, I used to work as a backend developer for a few years.'
		}
	}
}
</script>