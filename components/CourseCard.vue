<script setup>
defineProps({
  course: {
    type: Object,
    required: true,
    default: {}
  }
})
</script>

<template>
  <div class="card">
    <img :src="course.img" alt="">
    <div class="card__info">
      <h3 class="card__info-title">
        {{ course.title }}
      </h3>
      <p class="card__info-text">
        {{ course.text }}
      </p>
      <nuxt-link to="/" class="card__info-link"> Подробнее </nuxt-link>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  max-width: 300px;
  background: rgb(210, 210, 210);
  padding: 10px;
  border-radius: 5px;
  cursor: pointer;
  text-align: center;
  transition: .3s;

  &:hover {
    transform: scale(1.1);
  }


  & img {
    width: 100%;
    border-radius: 5px;
  }
  
  &__info {
    &-title {
      text-transform: uppercase;
      margin-top: 20px;
    }

    &-text {
      margin-top: 10px;
    }

    &-link {
      padding: 10px;
      width: 100%;
      border: 1px solid black;
      display: inline-block;
      margin-top: 10px;
      font-size: 16px;
    }
  }
}
</style>