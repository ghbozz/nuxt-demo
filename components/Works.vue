<template>
  <div class="container flex">
    <div id="works" class="w-full">
      <Showcase />
      <div class="flex mb-4">
        <Work v-for="work in works" :work="work" />
      </div>
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
  .work {
    margin: 20px 10px 0px 10px;
  }

  .work:first-of-type {
    margin-left: 0px;
  }

  .work:last-of-type {
    margin-right: 0px;
  }
</style>