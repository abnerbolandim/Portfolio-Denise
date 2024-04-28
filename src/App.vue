<template>
  <Navbar/>
  <Withdrawal/>
  <Categories/>
  <Products/>
  <About/>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Withdrawal from './components/Withdrawal.vue';
import Categories from './components/Categories.vue';
import Products from './components/Products.vue';
import About from './components/About.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Withdrawal,
    Categories,
    Products,
    About,
  }
}
</script>

<style>
#app{
  overflow-x: hidden;
}
</style>
