<template>
  <article class="bg-grey-10 px-4 py-16">
    <div
      class="max-w-6xl mx-auto grid md:grid-rows-none grid-rows-2 md:grid-cols-2 gap-x-12 gap-y-8"
    >
      <section
        class="flex justify-center items-center w-full transform xs:scale-100 sm:scale-120 lg:scale-130 xl:scale-140"
      >
        <AboutMeGirlSvg />
      </section>
      <section class="flex flex-col justify-center w-full sm:p-10 md:p-0">
        <h2>About</h2>
        <UiUnderline color="bg-primary-5" />

        <p class="text-grey-5 mt-4">
          I am a developer by passion with a keen interest in technology. Beside
          challenging myself, I love learning new technologies and languages.
        </p>

        <p class="text-grey-5 mt-4">
          My journey began as a Software Engineer, where I worked as an
          Automation Engineer, diving into automation and gradually branching
          out into full-stack development. Over time, my natural interest in art
          and design, along with a curiosity for user interfaces, drew me
          towards frontend development and throughout I have looked towards
          automating tasks like testing, deployment and monitoring.
        </p>

        <p class="text-grey-5 mt-4">
          I moved to the Netherlands to start a new chapter alongside my
          husband. It has been filled with exploration, travel, and the thrill
          of working on my portfolio. I’m eager to continue growing my skills,
          collaborating, and work on challenging projects that truly resonate.
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
