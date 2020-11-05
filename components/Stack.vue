<template>
  <div id="tools" class="mt-10">
    <h5 class="text-center text-5xl mt-12">Tools</h5>
    <div id="stack" class="w-full pt-6">
      <img id="figma" src="~/assets/images/figma.png">
      <img id="nuxt" src="~/assets/images/nuxt.svg" />
      <img id="rails" class="pb-5" src="~/assets/images/rails.svg" />
      <img id="webflow" src="~/assets/images/webflow_full.svg" />
      <img id="shopify" src="~/assets/images/shopify.png" />
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
  #tools h5 {
    font-family: 'Amatic SC', cursive;
    font-weight: bolder;
    color: rgb(220, 220, 220);
  }

  #stack {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: -35px;
  }

  #stack img {
    height: 40px;
    margin: 0px 35px;
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
    height: 65px !important;
  }
</style>