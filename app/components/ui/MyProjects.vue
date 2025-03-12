<template>
  <article class="bg-primary-10 p-20">
    <div class="">
      <div class="mb-16 text-center">
        <h2
          class="text-grey-1 text-4xl leading-none tracking-[0.25rem] mb-3 capitalize"
        >
          My Projects
        </h2>
        <p class="text-grey-5">
          Latest applications I developed as fun projects and self learning.
        </p>
      </div>
      <div class="max-w-6xl mx-auto">
        <p v-if="error">Something went wrong. Please try again later.</p>

        <template v-else-if="projectsInfo">
          <div
            v-for="(project, index) in projectsInfo?.projects"
            :key="project.id"
          >
            <section class="grid grid-cols-12 mb-16 items-center relative">
              <div
                class="row-start-1 col-span-full h-[32rem] p-16 bg-gradient-to-bl from-primary-6 to-gradient-1 rounded-md shadow-lg"
                :class="
                  index % 2 === 0
                    ? 'md:col-start-1 md:col-span-8'
                    : 'md:col-start-5 md:col-span-8'
                "
              >
                <img
                  :alt="project.title"
                  :src="project.image"
                  class="w-full h-full hover:opacity-100 object-fill"
                />
              </div>
              <UiProjectInfo
                :project="project"
                :class="
                  index % 2 === 0
                    ? 'md:col-start-5 md:col-span-8'
                    : 'md:col-start-1 md:col-span-8'
                "
              />
            </section>
          </div>
        </template>
        <p v-else>Loading...</p>
      </div>
    </div>
  </article>
</template>

<script setup>
const { error, data: projectsInfo } = await useFetch('/projects.json', {
  lazy: true,
  server: false,
  key: 'data-fetch',
});
</script>
