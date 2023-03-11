<template>
	<nav class="navbar center navbar-expand-lg navbar-dark bg-dark rounded">
	  <div class="collapse navbar-collapse d-flex justify-content-center" id="navbarSupportedContent">
	    <ul class="navbar-nav mr-auto">
	      <li class="nav-item" v-for="section in sections">
	        <a class="nav-link" :href="section.id">
	        	{{ section.text }}
	        </a>
	      </li>
	    </ul>
	  </div>
	</nav>
</template>

<script>
export default {
	data(){
		return{
			sections:[
				{
					'text':'About',
					'id':'#about'
				},
				{
					'text':'CV',
					'id':'#academic-cv'
				},
				{
					'text':'Experience',
					'id':'/experience'
				},
				{
					'text':'Publications',
					'id':'/publication'
				},
				{
					'text':'Teaching Assistant',
					'id':'https://teacher-assistant.github.io'
				},
				{
					'text':'Contact',
					'id':'#contact'
				}
			]
		}
	}
}
</script>