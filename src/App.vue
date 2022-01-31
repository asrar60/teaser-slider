<template>
  <div class="">
    <div class="teaser-slider mt-40">
      <!-- <div id="overlay"></div> -->
      <div class="flex mx-5 items-center text-teal-600">
        <h1 class="text-3xl font-bold ">Länder, Regionen, Orte</h1>
        <a class="ml-auto mr-3 text-2xl" href="#" title="alle-laender">Alle</a>
      </div>
      <h2 class="ml-5 text-lg">Lorem Ipsum Länder, Regionen, Orte</h2>
      <teaser-slider>
        <teaser-slider-card></teaser-slider-card>
      </teaser-slider>
       <ul class="wrapper" style="width:100%;height:100%;">
         <li v-for="card in cards" :key="card" class="box rounded-2xl m-5 shadow-lg shadow-lime-500" style="width:80%;height:80%;contain: paint; box-shadow: -2px 2px #D9E15F;">
              <a :href="card.link"> 
                <img class="" style="width:100%;height:100%;" :src="card.image" :alt="card.text">
              </a>
              <div class=" flex px-2 items-center h-12">
                <span class="text-teal-600 text-xl font-bold">{{card.text}}</span>
                <span class="ml-auto text-pink-900">
                  <span class="text-base">ab </span>
                  <span class="text-xl font-bold">€ {{card.price}}</span>
                </span>
              </div>
         </li>
       </ul>
    </div>
  </div>
</template>

<script>
import TeaserSlider from './components/TeaserSlider.vue';
import TeaserSliderCard from './components/TeaserSliderCard.vue';


export default {
  name: 'App',
  components: {
    TeaserSlider,
    TeaserSliderCard,
  },
  data() {
    return {
      cards: [
        {
          "text": "Ägypten",
          "price": 1237,
          "image": "https://images.flux.reisen/hotel/1262/1/s",
          "link": "https://google.com"
          },
          {
          "text": "Griechenland",
          "price": 334,
          "image": "https://images.flux.reisen/hotel/1262/1/s",
          "link": "https://google.com"
          },
          {
          "text": "Türkei",
          "price": 237,
          "image": "https://images.flux.reisen/hotel/1262/1/s",
          "link": "https://google.com"
          },
          {
          "text": "Italien",
          "price": 237,
          "image": "https://images.flux.reisen/hotel/1262/1/s",
          "link": "https://google.com"
          },
          {
          "text": "Spanien",
          "price": 379,
          "image": "https://images.flux.reisen/hotel/1262/1/s",
          "link": "https://google.com"
          },
          {
          "text": "Kroatien",
          "price": 88,
          "image": "https://images.flux.reisen/hotel/1262/1/s",
          "link": "https://google.com"
          },
          {
          "text": "Österreich",
          "price": 0,
          "image": "https://images.flux.reisen/hotel/1262/1/s",
          "link": "https://google.com"
          }
      ],
    }
  }
}


</script>

<style src="./assets/tailwind.css" > 

</style>
