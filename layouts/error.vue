<template>
  <div>
    <div>
      <div v-if="error.statusCode === 404" class="container mx-auto flex flex-col items-center justify-center py-10">
        <img class="w-25 md:w-1/2" src="../assets/svg/404.svg" />
        <h1 class="font-mono text-xl font-bold my-7">
          This page was not found.
        </h1>
        <partials-button url="/" text="Take Me Home"></partials-button>
      </div>
      <div v-else class="container mx-auto flex flex-col items-center justify-center py-10">
        <img class="w-25 md:w-1/2" src="../assets/svg/error.svg" />
        <h1>An unexpected error occured!</h1>
        <partials-button url="/" text="Take Me Home"></partials-button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["error"],
  layout: "error", // you can set a custom layout for the error page
};
</script>