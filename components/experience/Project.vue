<template>
	<div>
		<div :class="cls">
			<div class="mb-0 alert d-flex justify-content-between" :class="project.class">
				<div class="d-grid gap-1" style="width:85%">
					<h4 class="alert-heading">
						<b>{{ project.role }}</b> at <b>{{ project.name }}</b>
					</h4>
					<p>
						{{ project.description }}
					</p>
					<span v-for="(destination, text, index) in project.links">
						<a :href="destination" class="text-decoration-none">
							{{text}}
						</a>
						<span v-if="index != Object.keys(project.links).length - 1">|</span>
					</span>
				</div>
				<div class="d-grid gap-1"  style="width:15%">
					<span class="d-flex justify-content-center">
						{{ project.from }} - {{ project.to }}
					</span>
					<span class="d-flex justify-content-center">
						<img v-show="project.image" class="rounded" :src="project.image" height="110" width="110" />
					</span>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	props:['project']
}
</script>