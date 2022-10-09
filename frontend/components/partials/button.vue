<template>
    <nuxt-link :to="url">
        <button class="rounded-full py-3 px-8 text-white bg-gray-800 hover:bg-gray-900 w-full md:max-w-xs">{{ text }}</button>
    </nuxt-link>
</template>

<script>

export default {

    props: { 
        url: String,
        text: String
    }

}

</script>