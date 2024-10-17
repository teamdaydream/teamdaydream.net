<script setup lang="ts">
useSeoMeta({
  title: 'Team はくちゅーむ | 公式サイト | ' + useRoute().meta.name,
  description: 'Team はくちゅーむはチーム内で開発したプロジェクトを公開・提供する活動をしているチームです！',
  ogTitle: 'Team はくちゅーむ | 公式サイト',
  ogDescription: 'Team はくちゅーむはチーム内で開発したプロジェクトを公開・提供する活動をしているチームです！',
  ogImage: '/icon.webp',
  twitterCard: 'summary_large_image',
})
</script>

<template>
  <div>
    <NuxtLayout>
      <NuxtRouteAnnouncer />
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>

<style>
.page-enter-active,
.page-leave-active {
  transition: all 0.4s;
}
.page-enter-from,
.page-leave-to {
  opacity: 0;
  filter: blur(1rem);
}
</style>