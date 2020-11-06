<template>
  <div class="work h-screen relative">
    <div class="infos text-center px-12 mb-16">
      <h4 class="text-4xl">{{ work.title }}</h4>
      <p>{{ work.description }}</p>
    </div>
    
    <div class="showcase" data-aos="fade-up" data-aos-once="false" data-aos-duration="1000">
      <div class="image rounded" :class="{translate: details}"
          :style="`background-image: url(${image('desktop')})`">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['work', 'index'],
  data() {
    return {
      details: false
    }
  },
  methods: {
    image(format) {
      if (this.work.images) {
        const directory = this.work.title.toLowerCase().replace(' ', '_')
        return require(`~/assets/images/works/${directory}/${format}.png`)
      }
    },
    technos() {
      return this.work.techs.join(' - ')
    }
  }
}
</script>

<style scoped>
  .work {
    position: relative;
  }

  .image {
    height: 45.3rem;
    background-color: rgb(240, 240, 240);
    background-position: top;
    background-size: cover;
    box-shadow: 0px 1px 30px -1px rgba(0,0,0,0.07);
    border-radius: 7px;
    transition: all .5s ease-out;
  }
</style>