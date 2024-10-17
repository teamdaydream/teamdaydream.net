<script setup lang="ts">
const props = defineProps({
  name: {
    type: String,
    required: true
  },
  description: {
    type: String,
    required: true
  },
  icon: {
    type: String,
    required: true
  },
  github: {
    type: String,
    required: true
  },
  twitter: {
    type: String,
    required: false
  }
})
</script>

<template>
  <div class="flex items-center border-2 border-gray-200 dark:border-gray-700 rounded-2xl p-5 m-5">
    <NuxtImg :src="icon" class="lg:h-[200px] h-[100px] rounded-full" />
    <div class="ml-5">
      <h1 class="text-blue-300 lg:text-4xl text-2xl font-bold">{{name}}</h1>
      <p>{{description}}</p>
      <UButton class="mt-3" icon="i-mdi-github" size="sm" color="primary" variant="solid" label="GitHub" @click="navigateTo(`https://github.com/${github}`, {external: true, open: {target: '_blank'}})"/>
      <UButton v-if="twitter" class="mt-3 ml-3" icon="i-mdi-twitter" size="sm" color="primary" variant="solid" label="X" @click="navigateTo(`https://x.com/${twitter}`, {external: true, open: {target: '_blank'}})" />
    </div>
  </div>
</template>

<style scoped>

</style>