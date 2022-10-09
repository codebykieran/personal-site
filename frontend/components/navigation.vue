<template>
    <nav class="relative pb-5 mb-5 border-b">
		<div class="flex flex-col md:flex-row items-center justify-between text-lg">
			<nuxt-link class="font-mono font-bold text-2xl" to="/"><span>&lt;codebykieran/&gt;</span></nuxt-link>
			<ul id="navbar" class="hidden md:flex space-x-6">
				<nuxt-link class="nav-link" to="/about">about</nuxt-link>
				<nuxt-link class="nav-link" to="/work">services</nuxt-link>
				<nuxt-link class="nav-link" to="/contact">contact</nuxt-link>
			</ul>
			<button id="menu-btn" :class="navOpen ? 'open' : ''" class="block hamburger mt-6 md:hidden focus:outline-none" @click="toggleNav">
				<span class="hamburger-top"></span>
				<span class="hamburger-middle"></span>
				<span class="hamburger-bottom"></span>
			</button>
			<div class="md:hidden">
				<div id="menu" :class="navOpen ? 'flex' : 'hidden'" class="absolute flex-col items-center border-2 border-yellow-600 self-end py-8 mt-10 space-y-6 font-semibold bg-white sm:w-auto sm:self-center left-0 right-0">
					<nuxt-link class="nav-link" @click.native="toggleNav" to="/about">story</nuxt-link>
					<nuxt-link class="nav-link" @click.native="toggleNav" to="/work">services</nuxt-link>
					<nuxt-link class="nav-link" @click.native="toggleNav" to="/contact">contact</nuxt-link>
				</div>
			</div>
		</div>   
	</nav>
</template>

<script>
    export default {
		data() {
			return {
				navOpen: false,
			}
		},
		methods: {
			toggleNav() { 
				this.navOpen = !this.navOpen
			}
		}
    }
</script>

<style scoped>

.hamburger {
	cursor: pointer;
	width: 24px;
	height: 24px;
	transition: all 0.25s;
	position: relative;
}

.hamburger-top,
.hamburger-middle,
.hamburger-bottom {
	position: absolute;
	top: 0;
	left: 0;
	width: 24px;
	height: 2px;
	background: orange;
	transform: rotate(0);
	transition: all 0.5s;
}

.hamburger-middle{
	transform: translateY(7px);
}

.hamburger-bottom{
	transform: translateY(14px);
}

.open {
	transform: rotate(90deg);
	transform: translate(0px);
}

.open .hamburger-top {
	transform: rotate(45deg) translateY(6px) translate(6px); 
}

.open .hamburger-middle {
	display: none;
}

.open .hamburger-bottom {
	transform: rotate(-45deg) translateY(6px) translate(-6px); 
}

#menu {
	background: rgba(255, 255, 255, .95);
}


</style>

