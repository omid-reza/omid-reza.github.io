<template>
	<div id="submitted">
		<h3 class="text-light">
			Submitted works
		</h3>
		<div v-for="pub in pubs">
			<PublicationInformation :pub='pub' :cls='"alert alert-info"' />
		</div>
	</div>
</template>

<script>
export default {
	props:['pubs']
}
</script>