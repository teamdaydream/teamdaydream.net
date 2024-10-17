<script setup lang="ts">
// You can find emojis from https://animated-fluent-emoji.vercel.app/

defineProps({
  id: {
    type: String,
    required: true
  }
})
</script>

<template>
  <NuxtImg :src="`https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/${id}`" alt="emoji"/>
</template>

<style scoped>

</style>