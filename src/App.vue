<template>
  <div>
    <img class="icon" src="./assets/icon-star.svg">
    <cardRating msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import cardRating from './components/cardRating.vue'

export default {
  name: 'App',
  components: {
    cardRating
  }
}
</script>

<style>
#app {
  font-family: Overpass, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}


</style>
