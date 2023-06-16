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
			submitted:[],
			inPreparation:[],
			inProgress:[]
		}
	}
}
</script>
