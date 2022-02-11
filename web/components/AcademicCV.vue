<template>
	<div id="academic-cv">
		<div class="alert alert-primary">
			<div class="display-6">
				Academic Curriculum Vitae
			</div>
			<div class="container pt-1">
				You can download my academic curriculum vitae in diffrent formats from below links:
			</div>
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
					'link':'#'
				},
				'doc':{
					'text':'DOC',
					'link':'#'
				}
			}
		}
	}
}
</script>