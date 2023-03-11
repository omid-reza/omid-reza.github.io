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
			'text':'Omid Reza Heidari completed his undergraduate study at Islamic Azad University (Zanjan branch). He acted as a teaching assistant (TA) at several universities, namely Sharif University of Technology, Zanjan University, and Islamic Azad University. His area of interest contains databases, machine learning, deep learning, and data visualization. Moreover, He has participated as a researcher in machine learning and signal processing areas at Zanjan University of Medical Sciences.'
		}
	}
}
</script>