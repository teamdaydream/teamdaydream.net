<script setup lang="ts">
const colorMode = useColorMode()
const emoji = computed(() => colorMode.value === 'light' ? 'Travel%20and%20places/Sun%20with%20Face.png' : 'Travel%20and%20places/First%20Quarter%20Moon%20Face.png')
function switchTheme() {
  colorMode.preference
}
</script>

<template>
  <div>
    <button
        class="p-3"
        @click="colorMode.preference = (colorMode.value === 'light' ? 'dark' : 'light')">
      <FluentEmoji :id="emoji" class="w-7 h-7" />
    </button>
  </div>
</template>

<style scoped>

</style>