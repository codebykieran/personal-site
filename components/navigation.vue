<template>
    <nav class="relative pb-5 mb-5 border-b">
		<div class="flex items-center justify-between text-lg">
			<nuxt-link class="font-mono font-bold text-2xl" to="/"><span>&lt;codebykieran/&gt;</span></nuxt-link>
			<ul id="navbar" class="hidden md:flex space-x-6">
				<nuxt-link class="nav-link" to="/">home</nuxt-link>
				<nuxt-link class="nav-link" to="/about">about</nuxt-link>
				<nuxt-link class="nav-link" to="/work">work</nuxt-link>
				<nuxt-link class="nav-link" to="/contact">contact</nuxt-link>
			</ul>
		</div>   
	</nav>
</template>

<script>
    export default {
        
    }
</script>

