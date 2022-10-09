<template>
    <div class="flex flex-col-reverse md:flex-row align-center justify-between">
        <div class="flex flex-col space-y-6 align-center justify-center md:w-6/12 lg:w-6/12">
            <h1 class="font-mono text-4xl md:text-4xl lg:text-6xl font-light">Front-End Developer</h1>
            <span class="text-base lg:text-lg">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore deleniti, facilis laborum dolor molestiae ratione ipsa. Natus ullam odit delectus tempore, veritatis enim, quisquam libero dolorum ad consequatur minus est, commodi sunt earum quia nulla porro officiis perspiciatis eligendi? Officia molestiae inventore qui distinctio? Praesentium id asperiores nulla pariatur dolorem neque aperiam ipsam, saepe accusamus odio reprehenderit quas eligendi?</span>
            <partials-button url="/about" text="Discover More"></partials-button>
        </div>
        <img src="../../assets/svg/programming.svg" class="w-10/12 md:w-4/12 lg:w-5/12 mx-auto md:mx-0 py-12">
    </div>
</template>

<style scoped>

h1::after {
    content: '_';
    margin-left: .5rem;
    animation: 
        blinking .5s step-end infinite;
}

</style>