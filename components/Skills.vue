<template>
  <div class="container flex">
    <div id="skills" class="w-full">

      <div id="main-value" class="w-full rounded" data-aos="fade-up" data-aos-once="true" data-aos-duration="1000">
        <div class="infos text-right">
          <h4 class="text-4xl font-semibold">Main Value</h4>
          <p>Some Description</p>
        </div>
      </div>

      <div class="flex mb-4">
        <Skill :title="'Prototyping'" 
               :description="'Some Description'"
               :color="'rgb(199, 146, 233)'"
               :animation="'fade-right'"
               :delay="'200'"
               :duration="'1000'"/>

        <Skill :title="'Backend-Development'" 
               :description="'Some Description'"
               :color="'rgb(34, 34, 34)'"
               :animation="'fade-up'"
               :delay="'400'"
               :duration="'1000'"/>

        <Skill :title="'Frontend-Development'" 
               :description="'Some Description'"
               :color="'rgb(130, 170, 255)'"
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
  #main-value {
    height: 28rem;
    background-color: rgb(195, 232, 141);
    box-shadow: 0px 1px 30px -1px rgba(0,0,0,0.05);
    position: relative;
  }

  #main-value .infos {
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