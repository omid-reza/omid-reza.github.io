<template>
	<div id="InPreparation">
		<h3 class="text-warning">
			Works in preparation
		</h3>
		<div v-for="pub in pubs">
			<PublicationInformation :pub='pub' />
		</div>
	</div>
</template>

<script>
export default {
	props:['pubs']
}
</script>