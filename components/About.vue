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
			'text':'Omid Reza Heidari concluded his undergraduate studies at Islamic Azad University, Zanjan branch. He was a teaching assistant (TA) at several universities, namely Sharif University of Technology, Zanjan University, and Islamic Azad University, Zanjan branch. His area of interest includes machine learning, deep learning, databases, and data visualization. Furthermore, He has participated as a researcher in machine learning and signal processing areas at Zanjan University of Medical Sciences.'
		}
	}
}
</script>