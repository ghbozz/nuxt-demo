<template>
  <div id="stack" class="w-full">
    <img id="figma" src="~/assets/images/figma.png">
    <img id="rails" class="pb-3" src="~/assets/images/rails.svg" />
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
    height: 40px;
    margin: 0px 50px;
    filter: grayscale(15%);
  }

  #figma {
    height: 90px !important;
  }

  #rails {
    height: 170px !important;
  }

  #nuxt {
    height: 30px !important;
  }

  #shopify {
    height: 190px !important;
  }
</style>