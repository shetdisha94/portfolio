<template>
  <section>
    <BaseSection heading="Contact">
      <template #illustration>
        <ContactMeGirlSvg />
      </template>
      <template #content>
        <p class="text-grey-5 mt-4">
          Let's get to know each other, or just drop me a line.
        </p>

        <p class="text-grey-5 mt-4">
          If you are looking to get a hold of me, you can drop me a message:
        </p>
        <ul class="p-4">
          <li class="flex items-center gap-3 p-1">
            <EmailSvg />
            <a
              class="text-grey-1 font-bold tracking-[0.25rem] hover:text-primary-5 transition-colors duration-300 ease-in-out"
              target="_blank"
              rel="noopener noreferrer"
              href="mailto:shetdisha94@gmail.com"
              >shetdisha94@gmail.com</a
            >
          </li>
        </ul>

        <p class="mt-4">
          You can also reach out to me on any social media below.
        </p>
      </template>
    </BaseSection>
  </section>
</template>

<script setup lang="ts">
import BaseSection from '~/components/ui/BaseSection.vue';
import ContactMeGirlSvg from '~/assets/icons/svg/ContactMeGirlSvg.vue';
import EmailSvg from '~/assets/icons/svg/EmailSvg.vue';
</script>
