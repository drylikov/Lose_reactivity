<script setup lang="ts">
  const title = ref('My App Title')
  title.value = 'Another title'
</script>

<template>
  <div>
    <AppTitle :title="title" />
    <input v-model="title">
  </div>
</template>