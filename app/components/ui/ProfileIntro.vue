<template>
  <div class="@container/profile bg-primary-10">
    <div class="max-w-6xl mx-auto min-h-custom flex px-12 sm:px-20 pb-20">
      <article class="flex min-h-custom flex-col justify-center w-full">
        <UiUnderline color="bg-primary-5" />
        <h1>I'm Disha</h1>
        <h4 class="text-grey-5">
          Software <span class="xs:hidden">Dev</span>
          <span class="hidden xs:inline-block">Developer</span> By Passion
        </h4>

        <div class="mt-5">
          <UiLink label="Contact Me" type="primary" to="/contact" />
        </div>

        <div class="mt-10">
          <UiSocialActions />
        </div>
      </article>
      <article
        class="hidden md:flex justify-center items-center w-full transform xs:scale-90 sm:scale-100 lg:scale-120 xl:scale-140"
      >
        <HelloGirlSvg />
      </article>
    </div>
  </div>
</template>

<script setup lang="ts">
import HelloGirlSvg from '~/assets/icons/svg/HelloGirlSvg.vue';
</script>

<style scoped>
.min-h-custom {
  @apply min-h-[calc(100vh-5rem)];
}
</style>
