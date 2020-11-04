<template>
  <div>
    <Banner />
    <div class="min-h-screen pt-24 pb-4 bg-gradient">
      <Skills />
      <Stack />
    </div>
    <div class="min-h-screen py-4">
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

.bg-gradient {
  background: rgb(247,250,252);
  background: linear-gradient(90deg, 
              rgba(247,250,252,1) 0%, 
              rgba(244,244,244,1) 40%, 
              rgba(244,244,244,1) 60%, 
              rgba(247,250,252,1) 100%);
}
</style>
