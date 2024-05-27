<template>
    <q-page padding>
      <Carousel />
      <div class="q-pa-md">
        <q-card-deck>
          <ProductCard v-for="product in products" :key="product.id" :product="product" />
        </q-card-deck>
      </div>
    </q-page>
  </template>
  
  <script>
  import Carousel from '../components/Carousel.vue';
  import ProductCard from '../components/ProductCard.vue';
  
  export default {
    name: 'HomePage',
    components: {
      Carousel,
      ProductCard
    },
    data() {
      return {
        products: [
          { id: 1, name: 'Product 1', price: '$10', image: 'path/to/product1.jpg' },
          { id: 2, name: 'Product 2', price: '$20', image: 'path/to/product2.jpg' },
          { id: 3, name: 'Product 3', price: '$30', image: 'path/to/product3.jpg' }
        ]
      };
    }
  };
  </script>