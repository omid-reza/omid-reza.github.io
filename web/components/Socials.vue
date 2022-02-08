<template>
	<div class="alert alert-info">
		<div class="d-flex justify-content-center">
      		<a class="px-3" v-for="section in sections" :href="section.link">
				<box-icon type='logo' :name="section.class_name" size='lg' @mouseenter="changeColor(section)" @mouseleave="changeColor(section)" :color="[section.is_active ? section.color : '']" />
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
					is_active:false,
					color:'#BB001B',
					class_name:'gmail',
					link:'mailto:omid77.orh@gmail.com'
				},
				linkedin:{
					is_active:false,
					color:'#2867b2',
					class_name:'linkedin',
					link:'https://www.linkedin.com/in/omid-reza-heidari-30854a214/'
				},
				github:{
					is_active:false,
					color:'#333',
					class_name:'github',
					link:'https://www.github.com/omid-reza'
				},
				stackoverflow:{
					is_active:false,
					color:'#f48024',
					class_name:'stack-overflow',
					link:'https://stackoverflow.com/users/11215840/omid-reza'
				},
				twitter:{
					is_active:false,
					color:'#1da1f2',
					class_name:'twitter',
					link:'https://twitter.com/omid_reza_'
				}
			}
		}
	},
	methods:{
		changeColor(section){
			section.is_active=!section.is_active
		}
	}
}
</script>