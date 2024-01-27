<template>
  <carousel :items-to-show="1" :wrap-around="true" class="car" autoplay="4000" >
    <slide v-for="slide in images" :key="slide">
      <img :src="slide" alt="Carousel Image" class="carousel-image">
    </slide>

    <template #addons>
      <navigation />
      <pagination />
    </template>
  </carousel>
</template>

<script>
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel'

export default {
  name: 'App',
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
  },
  data() {
    return {
      images: [
        require('../imagenes/I.jpg'),
        require('../imagenes/v1.jpg'),
        require('../imagenes/v2.jpg'),
        // Add more image paths as needed
      ],
    };
  },
};
</script>

<style scoped>
  .car {
    position: fixed;
    left: 0;
    background-color: rgba(0, 0, 0, 0.183);
    top: 15vh;
    width: 100vw;
  }

  .carousel-image {
    width: 100%; /* Set the desired width for your images */
    height: auto; /* Maintain the aspect ratio */
    object-fit: fill;
    max-height: 60vh;
  }
</style>
