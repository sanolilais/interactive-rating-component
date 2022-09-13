<template>
  <div class="container">
    <h1>How did we do?</h1>
      <p> Please let us know how we did with you support request.
      All feedbak is appreciated to help us improve our offering!
      </p>
   <button @click="click">Submit</button>
  </div> 
   
      
</template>

<script>
import cardStars from './cardStars.vue'
export default {
  name: 'cardRating',
  components: {
    cardStars
  },
  props: {
    msg: String
  }
}
</script>

<style scoped>
.container {
  background-color:  hsl(213, 19%, 18%);
  color: hsl(0, 0%, 100%);
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 600px;
  height: 300px;
}

.painel-rating {
  display: flex;
}


</style>
