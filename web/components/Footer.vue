<template>
	<div>
		<div class="alert alert-danger">
			<div class="d-flex justify-content-center">
				<span>
					Code and design by:
					<span class="alert-link">
						who do you think?
					</span>
					  ©{{currentDate.getFullYear()}}
					Omid Reza Heidari.
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