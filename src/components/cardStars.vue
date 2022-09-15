<template>
  <div class="rating">
    <div id="rating__stars">
      <button @click="evaluate(1)" class="btn__evaluate"><i class="fa-regular fa-star"></i></button>
      <button @click="evaluate(2)" class="btn__evaluate"><i class="fa-regular fa-star"></i></button>
      <button @click="evaluate(3)" class="btn__evaluate"><i class="fa-regular fa-star"></i></button>
      <button @click="evaluate(4)" class="btn__evaluate"><i class="fa-regular fa-star"></i></button>
      <button @click="evaluate(5)" class="btn__evaluate"><i class="fa-regular fa-star"></i></button>
    </div>
  </div>
  <div id="rating__feedback" v-show="!status.feedback">
    <h1>Thank you!</h1>
    <p>We appreciate you taking the time to give a rating. If you ever need more support, dont hesitate to get in
      touch!
    </p>
    <p>Voce selecionou: {{starsRating}} out of 5</p>
  </div>
</template>

<style>
.rating__stars {
  margin-top: -22px;
}

.btn__evaluate {
  border-radius: 50px;
  width: 55px;
  height: 50px;
  background-color: hsl(213, 19%, 18%);
  border: none;
  cursor: pointer;
}

.btn__evaluate :hover {
  background-color: hsl(25, 97%, 53%);
  border: none;
}

.fa-star {
  width: 40px;
  height: 30px;
  color: hsl(60, 86%, 59%);
}
</style>

<script>
export default {
  data() {
    return {
      starsRating: 1,
      status: {
        feedback: true,
      }
    }
  },

  methods: {
    evaluate(num) {
      this.starsRating = num
      this.status = 'feedback'
    }
  }
}
</script>
