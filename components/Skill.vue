<template>
  <div class="skill w-1/3 overflow-hidden rounded"
       :style="'background-color:' + color" 
       data-aos-easing="ease-in-out" 
       data-aos-once="true"
       :data-aos="animation" 
       :data-aos-delay="delay"
       :data-aos-duration="duration">

    <div class="infos text-right">
      <h4 class="text-3xl font-semibold"
          data-aos="fade"
          data-aos-easing="ease-in-out" 
          data-aos-once="true"
          :data-aos-delay="delay"
          :data-aos-duration="duration">{{ title }}</h4>
      <p>{{ description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ['title', 'description', 'color','animation', 'delay', 'duration']
}
</script>

<style>
  .skill {
    color: white;
  }
</style>