<script setup>
const courses = [
  { img: '@/assets/images/programm.png', title: 'Веб Программирование', text: 'Создание сайтов и веб приложений' },
  { img: '@/assets/images/smm.png', title: 'Интернет Маркетинг', text: 'SMM и реклама в соц сетях' },
  { img: '@/assets/images/drop.png', title: 'Дропшиппинг', text: 'Работа с рынками Китая' },
]
</script>

<template>
  <div class="courses">
    <div class="courses__content container">
      <course-card v-for="course in courses" :key="course.img" :course="course" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.courses {
  &__content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;

    @media (max-width: 992px) {
      justify-content: center;
    }
  }
}
</style>