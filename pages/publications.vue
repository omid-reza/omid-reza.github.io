<template>
	<div class="container d-grid gap-2">
    	<div></div>
		<PublicationsCard />
		<PublicationsSubmitted :pubs='submitted' v-if="submitted.length"/>
		<PublicationsInPreparation :pubs='inPreparation' v-if="inPreparation.length"/>
		<PublicationsInProgress :pubs='inProgress' v-if="inProgress.length"/>
		<Footer />
	</div>
</template>

<script>
export default {
	data(){
		return{
			submitted:[
				{
					'title':'Assessment of structural connectivity and brain volumes after tDCS in stroke: a machine-learning method',
					'authors':[
						'Mohsen Dadashi',
						'Mehdi Maghbooli',
						'Ahmadreza Zakerian Zadeh',
						'Mohammad Soltani',
						'Mohammad Bayat',
						'Omid Reza Heidari'
					],
					'links':{
						'code':'https://github.com/omid-reza/StrokeMachineLearning'
					}
				}
			],
			inPreparation:[
				{
					'title':'Effectiveness of tDCS over the DLPFC on reducing clinical symptoms, improving working memory, and aberrant EEG functional connectivity in resting-state schizophrenia patients',
					'authors':[
						'Michael Nitsche',
						'Farahnaz Yousefi',
						'Mohsen Dadashi',
						'Omid Reza Heidari'
					],
					'links':{
						'code':'https://github.com/omid-reza/EEG'
					}
				}
			],
			inProgress:[]
		}
	}
}
</script>
