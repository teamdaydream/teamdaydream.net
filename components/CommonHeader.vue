<script setup lang="ts">
const items = [
  {
    name: 'ホーム',
    emoji: 'Travel%20and%20places/House.png',
    to: '/'
  },
  {
    name: '私達について',
    emoji: 'Symbols/White%20Exclamation%20Mark.png',
    to: '/about'
  },
  {
    name: 'メンバー紹介',
    emoji: 'People/Person.png',
    to: '/members'
  }
]

const mobileMenuToggle = ref(false)
</script>

<template>
  <header class="border-b-2 border-b-gray-100 dark:border-b-gray-800 py-2 flex">
    <div class="w-full max-w-[1400px] flex items-center mx-auto">
      <HeaderItem v-for="item in items" :name="item.name" :emoji="item.emoji" :to="item.to" class="hidden lg:block"/>
      <ThemeSwitcher class="ml-auto"/>
      <UButton :padded="false" variant="ghost" color="gray" icon="i-heroicons-bars-3" class="p-3 lg:hidden" @click="mobileMenuToggle = !mobileMenuToggle"/>
    </div>
  </header>
  <USlideover v-model="mobileMenuToggle" class="lg:hidden">
    <div class="p-4 flex-1">
      <UButton
          color="gray"
          variant="ghost"
          size="sm"
          icon="i-heroicons-x-mark-20-solid"
          class="flex absolute end-5 top-5 z-10"
          square
          padded
          @click="mobileMenuToggle = false"
      />
      <h1 class="text-2xl text-primary font-bold">Team はくちゅーむ</h1>
      <HeaderItem v-for="item in items" :name="item.name" :emoji="item.emoji" :to="item.to" class="my-3"/>
    </div>
  </USlideover>
</template>

<style scoped>

</style>