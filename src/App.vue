<template>
  <div>
    <cardRating msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import cardRating from './components/cardRating.vue'
export default {
  name: 'App',
  components: {
    cardRating,
  }
}
</script>

<style>
#app {
  width: 1280px;
  background-color: hsl(0, 0%, 0%);
  height: 610px;
  font-family: Overpass, Helvetica, Arial, sans-serif;
  text-align: center;
  color: hsl(210, 29%, 24%);
}
</style>
