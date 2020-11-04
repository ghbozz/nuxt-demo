<template>
  <div>
    <div class="h-screen">
      <Banner />
      <Stack />
    </div>
    <div class="min-h-screen py-4 flex justify-center items-center">
      <Works />
    </div>
  </div>
</template>

<script>
export default {

};
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  margin: 0 auto;
}
</style>
