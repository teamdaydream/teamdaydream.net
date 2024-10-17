<script setup lang="ts">
definePageMeta({
  name: "メンバー紹介"
})
</script>

<template>
  <div class="h-[400px] xl:max-w-[1200px] lg:max-w-[800px] md:max-w-[700px] sm:max-w-[600px] w-full mx-auto px-10">
    <PageHeader title="メンバー紹介" description="チームのメンバーについて紹介します" emoji="People/Person.png"/>
    <Member name="りや" description="Web関係メインでやってます。アマチュアだけど自宅サーバーも構築してます! 低レイヤーな部分も書いてみたい。" icon="/member-icon/riya.jpg" github="imriyaya" twitter="imriyaya"/>
    <Member name="res(るーず)" description="ゲーム開発に興味があります。まだまだ分からないことだらけですが楽しくプログラミング勉強中です！" icon="/member-icon/rse.jpg" github="rse00000" twitter="rse00000" />
    <Member name="蜜柑もち" description="得意領域は脆弱性テストなどのセキュリティ分野です！ 基本的に興味があれば何でも触ります。 最近だとDjangoを利用したWebなどなど...学習中です！" icon="/member-icon/mikanmochi.png" github="omochi05"/>
    <Member name="hiro_omochi1234" description="フロントエンドを勉強中... rustが最近のマイブーム java,python使ってます！" icon="/member-icon/hiro_omochi1234.png" github="hiro1234omochi"/>
  </div>
</template>

<style scoped>

</style>