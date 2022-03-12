<template>
	<div id="about">
		<div class="alert alert-success">
			<h3 class="alert-heading">
				About Me
			</h3>
			<p class="mb-0" v-html="text"></p>
		</div>
	</div>
</template>

<script>
export default {
	data(){
		return{
			'text':'I Have been studying software engineering since 2018. Also,i started programming when i was 17 years old with PHP and python, working with HTML and CSS to create static websites. <br /> Mainly build web applications as a web developer. Built applications with PHP and MySQL, Laravel, Vue.js, Nuxt.js, HTML5, CSS3, JavaScript. Apart from web, have python, Git and some NoSQL databases experience.'
		}
	}
}
</script>