<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>

<script setup lang="ts">
import { NuxtLayout } from '#components';

useHead({
  title: 'Disha Software Developer',
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
    {
      src: 'https://www.googletagmanager.com/gtag/js?id=G-ZZPXTZ4YV9',
    },

    {
      src: './gtag.js',
    },
  ],
});
</script>
