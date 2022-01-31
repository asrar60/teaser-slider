<template>
  <div class="">
    <div class="teaser-slider mt-40">
      <!-- <div id="overlay"></div> -->
      <div class="flex mx-5 items-center text-teal-600">
        <h1 class="text-2xl font-bold ">Länder, Regionen, Orte</h1>
        <a class="ml-auto mr-4 lg:mr-48 text-xl" href="#" title="alle-laender">Alle</a>
      </div>
      <h2 class="ml-5 text-lg">Lorem Ipsum Länder, Regionen, Orte</h2>
      <teaser-slider/>
    </div>
  </div>
</template>

<script>
  import TeaserSlider from './components/TeaserSlider.vue';

  export default {
    name: 'App',
    components: {
      TeaserSlider,
    }
  }
</script>

<style src="./assets/tailwind.css" > 

</style>
