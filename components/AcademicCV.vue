<template>
	<div id="academic-cv">
		<div class="alert alert-primary">
			<h3 class="alert-heading">
				Academic Curriculum Vitae
			</h3>
			<p class="mb-0">
				You can download my academic curriculum vitae in diffrent formats from below links:
			</p>
			<div class="d-flex justify-content-center pt-2">
				<div class="px-2" v-for="format in formats">
					<a type="button" class="btn btn-outline-primary" :href="format.link">
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
				'pdf':{
					'text':'PDF',
					'link':'https://omid-reza.github.io/CV.pdf'
				},
				'doc':{
					'text':'DOC',
					'link':'https://omid-reza.github.io/CV.docx'
				}
			}
		}
	}
}
</script>