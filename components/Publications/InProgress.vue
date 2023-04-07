<template>
	<div id="InPreparation">
		<h3 class="text-light">
			<img src="https://img.icons8.com/bubbles/1000/hand-with-pen.png" class="ico icon" />
			Works in Progress
		</h3>
		<div v-for="pub in pubs">
			<PublicationsInformation :pub='pub' :cls='"alert alert-secondary"' />
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
	props:['pubs']
}
</script>