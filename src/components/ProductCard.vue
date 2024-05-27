<template>
    <q-card>
      <q-img :src="product.image" />
      <q-card-section>
        <div class="text-h6">{{ product.name }}</div>
        <div>{{ product.price }}</div>
      </q-card-section>
      <q-card-actions align="right">
        <q-btn flat label="Add to Cart" color="primary" />
      </q-card-actions>
    </q-card>
</template>
  
<script>
  export default {
    name: 'ProductCard',
    props: {
      product: Object
    }
  };
</script>

<style scoped>
.product-card {
  width: 300px;
  margin: 1rem;
}
.q-img {
  height: 200px;
  object-fit: cover;
}
.q-card-section .text-h6 {
  font-weight: bold;
}
.text-subtitle2 {
  margin-top: 0.5rem;
}
</style>