<template>
  <section class="container">
    <div class="texts">
      <div class="icons">
        <img class="icon" src="../assets/icon-star.svg">
      </div>
      <h1>How did we do?</h1>
      <p class="description"> Please let us know how we did with you support request.
        All feedbak is appreciated to help us improve our offering!
      </p>
    </div>
    <cardStars />

    <button @click="click" class="btn-submit">Submit</button>
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
  height: 410px;
  border-radius: 40px;
  position: absolute;
  top: 20%;
  left: 30%;
  margin: -25px 0 0 -25px;
}

.icons {
  background-color: hsl(212.4, 33.3%, 21.8%);
  border-radius: 50px;
  width: 58px;
  height: 58px;
  margin-left: 40px;
}

.icon {
  margin: 19px;
  height: 20px;
}

.texts {
  text-align: left;
  margin: 25px;
  font-size: 15px;
}

h1 {
  margin-left: 30px;
}

.description {
  line-height: 28px;
  margin: auto 31px
}

.painel-rating {
  display: flex;
}

.btn-submit {
  width: 320px;
  background-color: hsl(25, 97%, 53%);
  height: 40px;
  border-radius: 20px;
  border: none;
  margin: 15px;
  cursor: pointer;
}

.btn-submit:hover {
  background-color: hsl(0, 0%, 100%);

}
</style>
