<template>
	<div id="InPreparation">
		<h3 class="text-light">
			<img src="https://img.icons8.com/bubbles/70/iphone-spinner.png" class="ico" />
			Works in Preparation
		</h3>
		<div v-for="pub in pubs">
			<PublicationsInformation :pub='pub' :cls='"alert alert-warning"'/>
		</div>
	</div>
</template>

<script>
export default {
	props:['pubs']
}
</script>