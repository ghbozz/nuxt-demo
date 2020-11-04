<template>
  <div id="works" class="container pt-12">
    <h3 class="text-center text-6xl">Recent works</h3>
    <Work v-for="work in works" :work="work"/>
  </div>
</template>

<script>
export default {
  data() {
    return {
      works: []
    }
  },
  async fetch() {
    this.works = await this.$content('works').sortBy('createdAt').fetch();
  }
}
</script>

<style>
  #works h3 {
    font-family: 'Amatic SC', cursive;
    font-weight: bolder;
  }
</style>