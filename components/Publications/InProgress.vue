<template>
	<div id="InPreparation">
		<h3 class="text-light">
			<img src="https://img.icons8.com/bubbles/70/hand-with-pen.png" class="ico" />
			Works in Progress
		</h3>
		<div v-for="pub in pubs">
			<PublicationsInformation :pub='pub' :cls='"alert alert-secondary"' />
		</div>
	</div>
</template>

<script>
export default {
	props:['pubs']
}
</script>