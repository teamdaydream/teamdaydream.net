<script setup lang="ts">

</script>

<template>
  <div class="background bg-cover py-10">
    <div class="h-[400px] xl:max-w-[1200px] lg:max-w-[800px] md:max-w-[700px] sm:max-w-[600px] w-full mx-auto flex items-center px-10 backdrop-blur-2xl sm:rounded-2xl rounded-none">
      <div>
        <h1 class="lg:text-6xl md:text-5xl sm:text-5xl text-3xl font-bold text-black">
          <div class="flex">
            Hello <p class="animate-pulse">👋</p>,
          </div>
          We're <span class="text-primary text-stroke">はくちゅーむ!</span>
        </h1>
        <p class="lg:text-xl text-sm text-black">
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
.background {
  background-image: url("/icon.webp");
  background-position: center center;
}

.text-stroke {
  -webkit-text-stroke: 2px rgba(62, 34, 2, 0.56);
}
</style>