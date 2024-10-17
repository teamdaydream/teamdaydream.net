<script setup lang="ts">
const props = defineProps({
  emoji: {
    type: String,
    required: true
  },
  name: {
    type: String,
    required: true
  },
  to: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="ml-10">
    <ULink :to="props.to" class="flex items-center">
      <FluentEmoji :id="emoji" class="w-7 h-7 mr-1" />
      <p class="text-primary font-bold">{{props.name}}</p>
    </ULink>
  </div>
</template>

<style scoped>

</style>