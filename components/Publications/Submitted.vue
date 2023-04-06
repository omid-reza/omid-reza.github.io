<template>
	<div id="submitted">
		<h3 class="text-light">
			<img src="https://img.icons8.com/bubbles/70/paper-plane.png" class="ico" />
			Submitted works
		</h3>
		<div v-for="pub in pubs">
			<PublicationsInformation :pub='pub' :cls='"alert alert-info"' />
		</div>
	</div>
</template>

<script>
export default {
	props:['pubs']
}
</script>