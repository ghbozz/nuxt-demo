<template>
  <div id="stack" class="w-full">
    <img id="rails" class="pb-3"src="~/assets/images/rails.svg" />
    <img id="nuxt" src="~/assets/images/nuxt.svg" />
    <img id="webflow" src="~/assets/images/webflow_full.svg" />
    <img id ="shopify" src="~/assets/images/shopify.svg" />
  </div>
</template>

<script>
export default {

}
</script>

<style>
  #stack {
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 20px 0px;
  }

  #stack img {
    height: 50px;
    margin: 0px 50px;
    filter: grayscale(15%);
  }

  #rails {
    height: 180px !important;
  }

  #nuxt {
    height: 40px !important;
  }

  #shopify {
    height: 200px !important;
  }
</style>