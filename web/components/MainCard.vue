<template>
    <div class="bg-warning rounded">
      <div class="d-grid gap-3 p-4 pb-0 pe-lg-0 pt-lg-5 rounded-3 shadow-lg">
        <div class="p-3 p-lg-5 pt-lg-3">
        	<div v-for="section in sections" class="alert" role="alert" @mouseenter="changeBgColor(section)" @mouseleave="changeBgColor(section)" :class="[section.is_active ? section.class_name : 'alert-dark']">
        		<h1 class="display-1 fw-bold lh-1">
        			{{ section.title }}
        		</h1>
        	</div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
	data(){
		return{
			sections:{
				full_name:{
					is_active: false,
					title:"Omid Reza Heidari",
					class_name: "alert-primary"
				},
				first_title:{
					is_active: false,
					title:"Software Engineer",
					class_name: "alert-warning"
				},
				second_title:{
					is_active: false,
					title:"Web Developer",
					class_name: "alert-danger"
				}
			}
		}
	},
  	methods:{
  		changeBgColor(section){
	  		section.is_active=!section.is_active
  		}
  	}
}
</script>