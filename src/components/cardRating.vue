<template>
  <section class="container">
    <h1>How did we do?</h1>
    <p> Please let us know how we did with you support request.
      All feedbak is appreciated to help us improve our offering!
    </p>
    <cardStars />
    <button @click="click">Submit</button>
  </section>
</template>

<script>
import cardStars from './cardStars.vue'
export default {
  name: 'cardRating',
  components: {
    cardStars
  },
}
</script>

<style scoped>
.container {
  background-color: hsl(213, 19%, 18%);
  color: hsl(0, 0%, 100%);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 500px;
  height: 365px;
  margin: 70px auto;
  border-radius: 40px;
}

.painel-rating {
  display: flex;
}

.btn-evaluate {
  border-radius: 50px;
  width: 60px;
  height: 60px;
  background-color: hsl(216, 11.3%, 43.3%);
}
</style>
