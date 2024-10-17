<script setup lang="ts">
const dateEvents: {date: string, emoji: string, description: string}[] = [
  {date: '2024/10/14', emoji: '🆕', description: 'チーム作成！'},
  {date: '2024/10/14', emoji: '🆙', description: 'rse(るーず)さんがチーム参加'},
  {date: '2024/10/16', emoji: '🆙', description: '蜜柑もち, hiro_omochi1234さんがチーム参加'}
]
</script>

<template>
  <div class="h-[400px] xl:max-w-[1200px] lg:max-w-[800px] md:max-w-[700px] sm:max-w-[600px] w-full mx-auto px-10">
    <PageHeader title="私達について" description="Team はくちゅーむについての説明です" emoji="Symbols/White%20Exclamation%20Mark.png" />
    <ul class="">
      <DateEvent v-for="dateEvent in dateEvents" :date="dateEvent.date" :emoji="dateEvent.emoji" :description="dateEvent.description" />
    </ul>
  </div>
</template>

<style scoped>

</style>