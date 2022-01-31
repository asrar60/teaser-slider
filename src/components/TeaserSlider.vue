<template>
       <ul class="wrapper flex lg:flex-col  " >
         <li v-for="card in cards" :key="card" class="box rounded-2xl m-5 w-4/5 h-full">
              <a :href="card.link"> 
                <img class="w-full h-full" :src="card.image" :alt="card.text">
              </a>
              <div class=" flex px-3 items-center h-12">
                <span class="text-teal-600 text-xl font-bold">{{card.text}}</span>
                <span class="ml-auto text-pink-900">
                  <span class="text-base">ab </span>
                  <span class="text-xl font-bold">€ {{card.price}}</span>
                </span>
              </div>
         </li>
       </ul>
</template>

<script>
export default {
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
            ]
        }
    }

}
</script>

<style src="../assets/tailwind.css" >

</style>