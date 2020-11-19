<template>
  <div id="contact-widget">
    <font-awesome-icon :icon="['fas', 'at']" @click="scrollDown($event)"/>
  </div>
</template>

<script>
export default {
  methods: {
    scrollDown(e) {
      document.querySelector('#footer').scrollIntoView({behavior: "smooth", block: "end"});
    }
  }
}
</script>

<style scoped>
  #contact-widget {
    position: fixed;
    bottom: 5%;
    right: 5%;
  }

  #contact-widget::after {
    position: absolute;
    transform: translate(-50%, -50%);
    left: 50%;
    top: 150%;
    content: '';
    width: 4px;
    height: 55px;
    background-color: rgb(30, 30, 30);
  }

  svg {
    font-size: 2.7rem;
    color: rgba(30, 30, 30);
    cursor: pointer;
  }
</style>