<template>
	<div class="alert alert-success" id="about">
		<h3 class="alert-heading">
			About Me
		</h3>
		<p class="mb-0" style="text-align: justify;" v-html="text"></p>
	</div>
</template>

<script>
export default {
	data(){
		return{
			'text':'Omid Reza Heidari is pursuing his master\'s studies in computer science at <a href="https://www.concordia.ca/" class="link-primary text-decoration-none">Concordia University</a>, advised by <a href="https://users.encs.concordia.ca/~wayang/" class="link-primary text-decoration-none">Professor Yang Wang</a>. Prior to that, he concluded his undergraduate studies at Islamic Azad University. He was a teaching assistant during his undergraduate studies at several universities, namely Sharif University of Technology, Zanjan University, and Islamic Azad University. His area of interest includes machine learning, deep learning databases, and data visualization.'
		}
	}
}
</script>

<style scoped>
a{

}
</style>