<template>
    <q-carousel v-model="slide" arrows navigation>
      <q-carousel-slide v-for="slide in slides" :key="slide.id" :name="slide.id" :img-src="slide.img" />
    </q-carousel>
</template>
  
<script>
  export default {
    name: 'Carousel',
    data() {
      return {
        slide: 1,
        slides: [
          { id: 1, img: 'path/to/image1.jpg' },
          { id: 2, img: 'path/to/image2.jpg' },
          { id: 3, img: 'path/to/image3.jpg' }
        ]
      };
    }
  };
</script>

<style scoped>
.carousel {
  height: 400px;
}
.q-carousel-slide {
  background-size: cover;
  background-position: center;
}
</style>