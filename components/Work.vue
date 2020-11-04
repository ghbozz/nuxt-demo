<template>
  <div class="work w-1/3 bg-indigo-200 overflow-hidden rounded">
    <div class="infos text-right">
      <h4 class="text-3xl font-semibold"
          data-aos="fade-left"
          data-aos-easing="ease-in-out" 
          data-aos-once="true"
          :data-aos-delay="work.index * 100"
          :data-aos-duration="work.index * 500">{{ work.title }}</h4>
      <p>{{ work.description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["work"]
}
</script>

<style>
  .work {
    position: relative;
    height: 24rem;
    box-shadow: 0px 1px 30px -1px rgba(0,0,0,0.05);
  }

  .work .infos {
    position: absolute;
    bottom: 20px;
    right: 20px;
  }
</style>