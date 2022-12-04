<script setup lang="ts">
const tags = [
  'Главная',
  'Посты',
  'Статьи',
  'Теги',
  'Темы',
  'Контакты',
]
</script>

<template>
  <div class="bg-black w-full h-full relative header relative py-7 h-96">
    <div class="flex flex-row justify-between items-center px-4 mx-auto max-w-7xl">
      <img src="./../assets/noemi-logo.svg" alt="Noemi-logo" class="w-[180px]">
      <div class="flex flex-row space-x-5">
        <a
          v-for="tag in tags"
          :key="tag"
          href="/"
          class="text-white uppercase"
        >
          {{ tag }}
        </a>
      </div>
    </div>
    <div class="absolute w-full h-full top-0 flex items-center justify-center">
      <h1 class="text-white  max-w-2xl text-center font-bold text-5xl">
        Блог о творчестве, спорте и образе жизни
      </h1>
    </div>
  </div>
</template>

<style scoped>
.header {
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url("./../assets/banner-bg.jpg");
  background-size: cover;
  background-position: center center;
  background-color: black;
}
</style>
