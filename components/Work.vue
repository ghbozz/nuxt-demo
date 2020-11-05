<template>
  <div class="work py-12">
    <div class="infos text-center px-12 mb-16">
      <h4 class="text-4xl">{{ work.title }}</h4>
      <p>{{ work.description }}</p>
    </div>
    <div class="card rounded"
         data-aos="fade-up" data-aos-once="true" data-aos-duration="1000"
         :style="`background-image: url(${image('desktop')})`">
    </div>
  </div>
</template>

<script>
export default {
  props: ['work', 'index'],
  methods: {
    image(format) {
      if (this.work.images) {
        return require(`~/assets/images/works/${this.work.title.toLowerCase()}/${format}.png`)
      }
    }
  }
}
</script>

<style scoped>
  .card {
    height: 45.3rem;
    background-color: rgb(240, 240, 240);
    background-position: top;
    background-size: cover;
    box-shadow: 0px 1px 30px -1px rgba(0,0,0,0.07);
    border-radius: 7px;
  }
</style>