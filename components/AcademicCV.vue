<template>
	<div id="cv">
		<div class="alert alert-primary">
			<h3 class="alert-heading">
				Curriculum vitae (CV)
			</h3>
			<p class="mb-0" style="text-align: justify;">
				My curriculum vitae is available and downloadable through the below link:
			</p>
			<div class="d-flex justify-content-center pt-2">
				<div class="px-2" v-for="format in formats">
					<a type="button" :class="format.class" :href="format.link">
						{{ format.text }}
					</a>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	data(){
		return{
			'formats':{
				'Academic CV':{
					'text':'Omid Reza\'s CV',
					'class':'btn btn-outline-danger',
					'link':'https://omid-reza.github.io/Omid Reza Heidari-CV.pdf'
				}
			}
		}
	}
}
</script>