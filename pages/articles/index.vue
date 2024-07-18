<script setup>
const { data } = await useAsyncData('articles', () => queryContent('articles').find())
</script>

<template>
  <div>
    <div>article</div>
    <pre>{{ data }}</pre>
  </div>
</template>
