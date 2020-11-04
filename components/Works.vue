<template>
  <div class="container">
    <div id="works">
      <Work v-for="work in works" :work="work" />
    </div>
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
    this.works = await this.$content('works').fetch();
  }
}
</script>

<style>

</style>