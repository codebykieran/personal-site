<template>
    <nav class="relative mb-5">
		<div class="flex items-center justify-between text-lg font-semibold">
			<nuxt-link to="/"><span>&lt;codebykieran/&gt;</span></nuxt-link>
			<ul class="hidden md:flex space-x-6">
				<nuxt-link to="about" class="">story</nuxt-link>
				<nuxt-link to="work" class="">work</nuxt-link>
				<nuxt-link to="contact" class="">contact</nuxt-link>
			</ul>
		</div>   
	</nav>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

</style>