<script setup lang="ts">

</script>

<template>
  <div>
    <div class="h-[400px] xl:max-w-[1200px] lg:max-w-[800px] md:max-w-[600px] sm:max-w-[500px] max-w-[400px] flex items-center mx-auto">
      <div>
        <h1 class="lg:text-6xl md:text-5xl sm:text-5xl text-3xl font-bold">
          Hello 👋,
          <br>
          We're <span class="text-primary">はくちゅーむ!</span>
        </h1>
        <p class="lg:text-xl text-sm">
          私達はチーム内で開発したプロジェクトを公開・提供する活動をしているチームです！
        </p>
        <div class="flex mt-5">
          <UButton class="font-bold" @click="navigateTo('/about')">About</UButton>
          <UButton class="font-bold ml-4" @click="navigateTo('/members')">メンバー紹介</UButton>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
</style>