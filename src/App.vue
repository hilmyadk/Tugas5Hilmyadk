<template>
  <q-layout>
    <NavBar />
    <q-page-container>
      <HomePage />
    </q-page-container>
    <Footer />
  </q-layout>
</template>

<script>
import NavBar from './components/NavBar.vue';
import HomePage from './views/HomePage.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    HomePage,
    Footer
  }
};
</script>

<style>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #6dccd8;
}
</style>