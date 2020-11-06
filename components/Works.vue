<template>
  <div id="works" class="container pt-16">
    <h3 class="text-center text-6xl mb-12">Recent works</h3>
    <h3 class="text-center text-6xl -m-16 mb-12">-</h3>
    <Work v-for="(work, index) in works" :work="work" :index="index" />
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
    this.works = await this.$content('works').sortBy('index', 'desc').fetch();
  }
}
</script>

<style>
  #works h3 {
    font-family: 'Amatic SC', cursive;
    font-weight: bolder;
  }
</style>