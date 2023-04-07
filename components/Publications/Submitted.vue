<template>
	<div id="submitted">
		<h3 class="text-light">
			<img src="https://img.icons8.com/bubbles/1000/paper-plane.png" class="ico icon" />
			Submitted works
		</h3>
		<div v-for="pub in pubs">
			<PublicationsInformation :pub='pub' :cls='"alert alert-info"' />
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