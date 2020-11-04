<template>
  <div id="showcase" class="w-full bg-green-200 rounded">
    <div class="infos text-right">
      <h4 class="text-4xl">{{ work.title }}</h4>
      <p>{{ work.description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      work: null
    }
  },
  async fetch() {
    const response = await this.$content('works')
                           .where({showcase: true})
                           .fetch();
    this.work = response[0]
  }
}
</script>

<style>
  #showcase {
    height: 28rem;
    box-shadow: 0px 1px 30px -1px rgba(0,0,0,0.1);
    position: relative;
  }

  #showcase .infos {
    position: absolute;
    right: 20px;
    bottom: 20px;
  }
</style>