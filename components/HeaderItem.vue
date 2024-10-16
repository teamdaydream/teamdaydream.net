<script setup lang="ts">
const props = defineProps({
  icon: {
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
      <UIcon class="w-5 h-5 mr-1" :name="props.icon"/>
      <p class="text-primary font-bold">{{props.name}}</p>
    </ULink>
  </div>
</template>

<style scoped>

</style>