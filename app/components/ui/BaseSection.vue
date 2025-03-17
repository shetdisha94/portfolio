<template>
  <article class="bg-primary-10 min-h-custom px-8 py-18">
    <div
      class="max-w-6xl mx-auto grid md:grid-rows-none md:grid-cols-2 gap-x-12 gap-y-8"
    >
      <figure
        class="flex justify-center items-center transform xs:scale-90 sm:scale-100 lg:scale-110 xl:scale-120"
      >
        <slot name="illustration"></slot>
      </figure>

      <section class="flex flex-col justify-center w-full">
        <h2>{{ heading }}</h2>

        <UiUnderline color="bg-primary-5 mb-2" />
        <slot name="content"></slot>
        <slot name="default"></slot>
        <div class="mt-10">
          <UiSocialActions />
        </div>
      </section>
    </div>
  </article>
</template>

<script setup lang="ts">
defineProps({
  heading: {
    type: String,
    required: true,
  },
});
</script>

<style scoped>
.min-h-custom {
  @apply min-h-[calc(100vh-5rem)];
}
</style>
