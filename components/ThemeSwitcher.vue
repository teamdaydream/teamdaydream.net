<script setup lang="ts">
const colorMode = useColorMode()
const icon = computed(() => colorMode.value === 'light' ? 'i-heroicons-sun' : 'i-heroicons-moon')
function switchTheme() {
  colorMode.preference
}
</script>

<template>
  <div>
    <UButton
        :padded="false"
        variant="ghost"
        color="gray"
        :icon="icon"
        class="p-3"
        @click="colorMode.preference = (colorMode.value === 'light' ? 'dark' : 'light')"
    />
  </div>
</template>

<style scoped>

</style>