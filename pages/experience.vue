<template>
	<div class="container d-grid gap-2">
    	<div></div>
		<experienceCard />
		<div v-for="project in projects">
			<experienceProject :project="project" />
		</div>
		<Footer />
	</div>
</template>

<script>
import 'boxicons'
export default {
	data(){
		return {
			projects:[
				{
					'name':'Hotel Motel',
					'class': 'alert-primary',
					'role':'Full Stack Developer',
					'from':'Aug 2021',
					'to':'Dec 2021',
					'image':'https://avatars.githubusercontent.com/u/89409106?s=200&v=4',
					'description':'Hotel Motel organization is a hotel-booking application consisting of three components: API, front-end, and collaborative recommender system. Moreover, this project has been developed via three web frameworks: Laravel, Nuxt.js,  and FastAPI.',
					'links':{
						'Code':'https://github.com/hotel-motel/'
					}
				},
				{
					'name':'Coffake',
					'class':'alert-danger',
					'role':'Full Stack Developer',
					'from':'Jun 2021',
					'to':'Feb 2022',
					'image':'https://avatars.githubusercontent.com/u/77469953?s=200&v=4',
					'description':'Coffake is a coffee delivery web application with two main components: API and Front-end. Furthermore, this project has been implemented via two web frameworks: Laravel and Nuxt.js.',
					'links':{
						'Code':'https://github.com/coffake/'
					}
				},
				{
					'name':'Cansell',
					'class':'alert-success',
					'role':'Back-end Developer',
					'from':'Apr 2020',
					'to':'Apr 2020',
					'image':'https://quera.org/media/CACHE/images/public/logos/98f94b3db0fa42b8b1ce841d2a543e8d/f6877d9272c2f2d5040bfeec23ee15ca.png',
					'description':'Participated in developing API that was based on Laravel.',
					'links':{
						'Website':'https://cansell.info/'
					}
				},
				{
					'name':'Onlinegnet',
					'class':'alert-danger',
					'role':'Back-end Developer',
					'from':'Oct 2019',
					'to':'Nov 2019',
					'description':'Participated in developing some novel features, such as renting games.'
				}
			]
		}
	}
}
</script>
