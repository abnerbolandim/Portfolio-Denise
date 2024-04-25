<template>
  <Navbar/>
  <Withdrawal/>
  <Categories/>
  <Products/>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Withdrawal from './components/Withdrawal.vue';
import Categories from './components/Categories.vue';
import Products from './components/Products.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Withdrawal,
    Categories,
    Products,
  }
}
</script>

<style>
#app{
  overflow-x: hidden;
}
</style>
