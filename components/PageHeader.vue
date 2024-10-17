<script setup lang="ts">
const props = defineProps({
  title: {
    type: String,
    required: true
  },
  description: {
    type: String,
    required: true
  },
  emoji: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="p-2">
    <div class="flex items-center">
      <FluentEmoji class="lg:h-16 md:h-14 sm:h-12 h-8" :id="emoji" />
      <h1 class="text-4xl text-primary font-bold">{{title}}</h1>
    </div>
    <p class="mt-5">{{description}}</p>
  </div>
</template>

<style scoped>

</style>