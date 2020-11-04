<template>
  <div class="container flex">
    <div id="works" class="w-full">
      <Showcase data-aos="fade-right" data-aos-once="true" data-aos-duration="1000" />
      <div class="flex mb-4">
        <Work v-for="work in works" :work="work" :key="work.index"
              data-aos-easing="ease-in-out" 
              data-aos="fade-up" 
              data-aos-once="true"
              :data-aos-delay="work.index * 100" 
              :data-aos-duration="work.index * 500" />
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
    this.works = await this.$content('works')
                           .sortBy('index')
                           .fetch();
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