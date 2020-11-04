<template>
  <div class="work w-1/3 bg-gray-400">
    {{ work.title }}
  </div>
</template>

<script>
export default {
  props: ["work"]
}
</script>

<style>
  .work {
    height: 24rem;
  }
</style>