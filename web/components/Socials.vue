<template>
	<div class="alert alert-info">
		<div class="d-flex justify-content-center">
      		<a class="px-3" v-for="section in sections" :href="section.link">
				<box-icon type='logo' :name="section.class_name" size='lg' />
	        </a>
      	</div>
	</div>
</template>

<script>
export default {
	data(){
		return{
			sections:{
				gamil:{
					class_name:'gmail',
					link:'mailto:omid77.orh@gmail.com'
				},
				linkedin:{
					class_name:'linkedin',
					link:'https://www.linkedin.com/in/omid-reza-heidari-30854a214/'
				},
				github:{
					class_name:'github',
					link:'https://www.github.com/omid-reza'
				},
				stackoverflow:{
					class_name:'stack-overflow',
					link:'https://stackoverflow.com/users/11215840/omid-reza'
				},
				twitter:{
					class_name:'twitter',
					link:'https://twitter.com/omid_reza_'
				}
			}
		}
	}
}
</script>