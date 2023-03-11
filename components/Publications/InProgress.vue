<template>
	<div id="InPreparation">
		<h3 class="text-light">
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