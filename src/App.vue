<template>
  <Navbar/>
  <Withdrawal/>
  <Categories/>
  <Products/>
  <About/>
  <Contact/>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Withdrawal from './components/Withdrawal.vue';
import Categories from './components/Categories.vue';
import Products from './components/Products.vue';
import About from './components/About.vue';
import Contact from './components/Contact.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Withdrawal,
    Categories,
    Products,
    About,
    Contact,
  }
}
</script>

<style>
#app{
  overflow-x: hidden;
}
</style>
