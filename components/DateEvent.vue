<script setup lang="ts">
defineProps({
  date: {
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
  <li>
    <div class="flex items-center my-3">
      <a class="text-4xl">{{emoji}}</a>
      <a class="ml-3 w-20 text-primary">{{date}}</a>
      <p class="ml-5">{{description}}</p>
    </div>
  </li>
</template>

<style scoped>

</style>