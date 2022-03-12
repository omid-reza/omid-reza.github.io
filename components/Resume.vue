<template>
	<div id="resume">
		<div class="alert alert-warning">
			<h3 class="alert-heading">
				Resume
			</h3>
			<p class="mb-0">
				You can download my resume in diffrent formats from below links:
			</p>
			<div class="d-flex justify-content-center pt-2">
				<div class="px-2" v-for="format in formats">
					<a type="button" class="btn btn-outline-dark" :href="format.link">
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
					'link':'https://omid-reza.github.io/Resume.pdf'
				},
				'doc':{
					'text':'DOC',
					'link':'https://omid-reza.github.io/Resume.docx'
				}
			}
		}
	}
}
</script>