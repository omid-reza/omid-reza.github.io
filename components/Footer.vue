<template>
	<div>
		<div class="alert alert-dark">
			<div class="d-flex justify-content-center">
				<span>
					@Copyright
					  {{currentDate.getFullYear()}}
					Omid Reza Heidari.
					Hosted by <a class="link-dark text-decoration-none" href="https://pages.github.com">GitHub Pages</a>.
				</span>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	data(){
		return{
			currentDate:new Date
		}
	}
}
</script>