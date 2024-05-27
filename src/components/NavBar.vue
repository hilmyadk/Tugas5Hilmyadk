<template>
    <q-header elevated class="bg-primary text-white">
      <q-toolbar>
        <q-btn flat round icon="menu" aria-label="Menu" @click="toggleDrawer"></q-btn>
        <q-toolbar-title>My Online Shop</q-toolbar-title>
      </q-toolbar>
    </q-header>
</template>
  
<script>
  export default {
    name: 'NavBar',
    methods: {
      toggleDrawer() {
        // Handle drawer toggle
      }
    }
  };
</script>

<style scoped>
.q-header {
  background-color: #027be3;
}
.q-toolbar-title {
  font-size: 1.5rem;
  font-weight: bold;
}
</style>