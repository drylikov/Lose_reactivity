<script setup lang="ts">
  const props = defineProps<{ title: string }>()

  /* similarity -> reactive getter
  watch(() => props.title, (title) => {
  })
  */

  useSeoMeta({
    title: () => props.title
  })
</script>

<template>
  <div>
    {{ title }}
  </div>
</template>