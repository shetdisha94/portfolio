<template>
  <article class="bg-grey-10 py-10">
    <div
      class="max-w-6xl mx-auto grid grid-rows-2 md:grid-rows-none md:grid-cols-2 gap-x-12 gap-y-8 md:py-8"
    >
      <section
        class="flex justify-center items-center w-full transform xs:scale-90 sm:scale-100 lg:scale-110 xl:scale-120"
      >
        <AboutMeGirlSvg />
      </section>
      <section class="flex flex-col justify-center w-full p-10 md:p-4">
        <h2>About</h2>
        <UiUnderline color="bg-primary-5" />

        <p class="text-grey-5 mt-4">
          I am a developer by passion with a keen interest in technology. Beside
          challenging myself, I love learning new technologies and languages.
        </p>

        <p class="text-grey-5 mt-4">
          An experienced and skilled Frontend Developer with over 4+ years of
          experience in crafting user-centric web applications. Specialized in
          web development with a strong passion for building highly efficient
          scalable web solutions. Motivated and demonstrated the ability to lead
          and collaborate with cross-functional teams to deliver high-quality
          software solutions.
        </p>

        <UiLink label="Learn More" type="primary" to="/contact" />
      </section>
    </div>
  </article>
</template>

<script setup lang="ts">
import AboutMeGirlSvg from '~/assets/icons/svg/AboutMeGirlSvg.vue';
</script>

<style scoped></style>
