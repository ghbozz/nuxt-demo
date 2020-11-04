<template>
  <div class="skill skill w-1/3 bg-indigo-200 overflow-hidden rounded" 
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
  props: ['title', 'description', 'animation', 'delay', 'duration']
}
</script>

<style>

</style>