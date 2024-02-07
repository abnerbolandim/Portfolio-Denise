<template>
  <Navbar/>
  <Withdrawal/>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Withdrawal from './components/Withdrawal.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Withdrawal,
  }
}
</script>

<style>

</style>
