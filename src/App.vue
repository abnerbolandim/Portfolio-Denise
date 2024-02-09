<template>
  <Navbar/>
  <Withdrawal/>
  <Categories/>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Withdrawal from './components/Withdrawal.vue';
import Categories from './components/Categories.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Withdrawal,
    Categories,
  }
}
</script>

<style>

</style>
