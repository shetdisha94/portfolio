<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>

<script setup lang="ts">
import { NuxtLayout } from '#components';

useHead({
  title: 'Disha Frontend Developer',
  meta: [
    {
      name: 'description',
      content: 'Community page',
    },
  ],
  script: [
    {
      src: './theme-toggle.js',
    },
  ],
});
</script>
