<template>
  <div id="contact-widget">
    <font-awesome-icon :icon="['fas', 'at']"/>
  </div>
</template>

<script>
export default {

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
    height: 50px;
    background-color: rgb(31, 31, 31);
  }

  svg {
    font-size: 3rem;
    color: rgb(31, 31, 31);
    cursor: pointer;
  }
</style>