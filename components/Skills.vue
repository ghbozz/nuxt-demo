<template>
  <div class="container flex">
    <div id="skills" class="w-full">

      <div id="showcase" class="w-full bg-green-200 rounded" data-aos="fade-up" data-aos-once="true" data-aos-duration="1000">
        <div class="infos text-right">
          <h4 class="text-4xl font-semibold">Title</h4>
          <p>Description</p>
        </div>
      </div>

      <div class="flex mb-4">
        <Skill :title="'hello'" 
               :description="'Some Description'"
               :animation="'fade-right'"
               :delay="'200'"
               :duration="'1000'"/>

        <Skill :title="'hello'" 
               :description="'Some Description'"
               :animation="'fade-up'"
               :delay="'400'"
               :duration="'1000'"/>

        <Skill :title="'hello'" 
               :description="'Some Description'"
               :animation="'fade-left'"
               :delay="'600'"
               :duration="'1000'"/>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
  #showcase {
    height: 28rem;
    box-shadow: 0px 1px 30px -1px rgba(0,0,0,0.05);
    position: relative;
  }

  #showcase .infos {
    position: absolute;
    right: 20px;
    bottom: 20px;
  }

  .skill {
    margin: 20px 10px 0px 10px;
    position: relative;
    height: 24rem;
    box-shadow: 0px 1px 30px -1px rgba(0,0,0,0.05);
  }

  .skill .infos {
    position: absolute;
    bottom: 20px;
    right: 20px;
  }

  .skill:first-of-type {
    margin-left: 0px;
  }

  .skill:last-of-type {
    margin-right: 0px;
  }
</style>