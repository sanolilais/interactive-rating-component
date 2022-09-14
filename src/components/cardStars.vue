<template>
  <div class="rating">
    <div class="painel-rating">
      <button @click="evaluate" class="btn-evaluate"><i class="fa-regular fa-star"></i></button>

      <button @click="evaluate" class="btn-evaluate"><i class="fa-regular fa-star"></i></button>

      <button @click="evaluate" class="btn-evaluate"><i class="fa-regular fa-star"></i></button>

      <button @click="evaluate" class="btn-evaluate"><i class="fa-regular fa-star"></i></button>

      <button @click="evaluate" class="btn-evaluate"><i class="fa-regular fa-star"></i></button>
    </div>
  </div>
</template>

<style>
.painel-rating {
  display: flex;
  flex-direction: row;
  justify-content: center;
  gap: 30px;
}

.btn-evaluate {
  border-radius: 50px;
  width: 60px;
  height: 60px;
  background-color: hsl(216, 12%, 54%);
  border: none;
}

.fa-star {
  width: 40px;
  height: 30px;
  color: rgb(240, 240, 60);
}
</style>

<script>

</script>
