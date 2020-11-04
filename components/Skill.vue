<template>
  <div class="skill w-1/3 overflow-hidden rounded"
       :style="'background-color:' + color" 
       data-aos-easing="ease-in-out" 
       data-aos-once="true"
       :data-aos="animation" 
       :data-aos-delay="delay"
       :data-aos-duration="duration">

    <div class="infos text-right"
         data-aos="fade"
         data-aos-easing="ease-in-out" 
         data-aos-once="true"
         :data-aos-delay="delay"
         :data-aos-duration="duration">
      <h4 class="text-3xl font-semibold">{{ title }}</h4>
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
    color: rgb(247, 250, 252);
  }
</style>