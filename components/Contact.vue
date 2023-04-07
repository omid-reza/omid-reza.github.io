<template>
	<div id="contact">
		<div class="alert alert-info">
			<div class="d-flex justify-content-center">
	      		<a class="px-3" v-for="section in sections" :href="section.link">
					<img class="ico icon" :src="section.source"/>
		        </a>
	      	</div>
		</div>
	</div>
</template>

<style>
.icon{
	width: 70px;
	height: 70px;
}	
</style>

<script>
export default {
	data(){
		return{
			sections:{
				gamil:{
					source: 'https://img.icons8.com/bubbles/2000/gmail-new.png',
					link:'mailto:omid77.orh@gmail.com'
				},
				linkedin:{
					source: 'https://img.icons8.com/bubbles/2000/linkedin.png',
					link:'https://www.linkedin.com/in/omid-reza-heidari-30854a214/'
				},
				github:{
					source: 'https://img.icons8.com/bubbles/2000/github.png',
					link:'https://www.github.com/omid-reza'
				},
				twitter:{
					source:'https://img.icons8.com/bubbles/2000/twitter-circled.png',
					link:'https://twitter.com/omid_reza_'
				},
				medium:{
					source: 'https://img.icons8.com/bubbles/2000/medium-new.png',
					link:'https://medium.com/@omidreza'
				},
				facebook:{
					source: 'https://img.icons8.com/bubbles/2000/facebook-new.png',
					link:'https://www.facebook.com/omidrezaheidari77'
				},
			}
		}
	}
}
</script>