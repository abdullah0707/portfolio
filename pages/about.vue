<template>
  <div class="custom-section mx-auto h-screen overflow-scroll">
    <div class="flex lg:flex-row max-lg:flex-col-reverse items-center">
      <div class="basis-1/2 max-lg:basis-3/4 text-white custem">
        <h1
          class="uppercase font-semibold flex text-4xl lg:text-2xl text-white max-sm:text-sm slide-in-top items-center">
          <div class="content__container">
            <div class="content__container__text text-flicker-in-glow">
              I am a Front-End
            </div>
            <ul class="content__container__list inline-block px-2">
              <li class="content__container__list__item leading-4">W E B</li>
              <li class="content__container__list__item leading-4">
                v u e . j s
              </li>
              <li class="content__container__list__item leading-4">
                n u x t . j s
              </li>
              <li class="content__container__list__item leading-4">
                D e v e l o p e r
              </li>
            </ul>
          </div>
        </h1>
        <div class="text-xl">
          <p class="p-3">
            Live in Egypt,Cairo. I have a serious passion for UI effects,
            creating intuitive, dynamic user experiences. Well-organised person,
            problem solver, independent employee with high attention to detail.
            I can professionally design and develop website interfaces using a
            framework or static code and also responsive to all screens and
            taking into account search engines.
          </p>
          <div class="flex justify-between max-lg:flex-col slide-in-bottom text-lg">
            <p class="text-yellow-400">
              <NuxtLink class="underlined underlined--right" target="_blank"
                to="https://drive.google.com/file/d/1z3GWygWifqJiJ_EcQQnrA_GLA1kSOV0q/view?usp=sharing">
                Download my latest CV
              </NuxtLink>
            </p>
            <p class="text-yellow-400">
              <NuxtLink class="underlined underlined--left" to="/contact">
                Contact with me
              </NuxtLink>
            </p>
          </div>
        </div>
      </div>
      <div class="basis-1/2 max-lg:basis-1/4 flex justify-center items-center slide-in-right z-0">
        <img class="w-6/12 max-w-min rounded-full max-md:m-5 bg-stone-500 user mb-6" src="../assets/image/p.jpg" />
      </div>
    </div>
    <h2 class="text-center font-semibold text-6xl text-white mb-4 mt-10 md:mt-10 lg:mt-0">
      MY skills
    </h2>
    <div class="flex lg:flex-row max-lg:flex-col items-center gap-10 w-full justify-between text-white">
      <div class="w-11/12 max-w-full">
        <p>
          Technical skills
        </p>
        <template v-for="technicalSkill in technicalSkills" :key="technicalSkill.name">
          <p class="label">
            <span class="effect-shine text-xl">
              {{ technicalSkill.name }}
            </span>
          </p>
          <UProgress class="my-2" color="white" :indicator="false" :value="technicalSkill.i" />
        </template>
      </div>
      <div class="w-11/12 max-w-full">
        <p>
          Personal Skills
        </p>
        <template v-for="personalSkill in personalSkills" :key="personalSkill.name">
          <p class="label">
            <span class="effect-shine text-xl">
              {{ personalSkill.name }}
            </span>
          </p>
          <UProgress class="my-2" color="white" :indicator="false" :value="personalSkill.i" />
        </template>
      </div>
    </div>
    <!-- <div class="overflow-visible relative max-w-fit min-w-fit mx-auto shadow-lg ring-1 ring-black/5 rounded-xl flex items-center gap-6 dark:bg-slate-800 dark:highlight-white/5">
         <img class="absolute -left-6 w-24 h-24 rounded-full shadow-lg" src="../assets/image/p.jpg">
         <div class="flex flex-col py-5 px-20">
            <strong class="text-slate-900 text-sm font-medium dark:text-slate-200 hover:uppercase">Abdallah Mohamed</strong>
            <span class="text-slate-500 text-sm font-medium dark:text-slate-400 hover:uppercase">Front-End Developer</span>
         </div>
      </div> -->
  </div>
</template>

<script setup>
useHead({
  titleTemplate: "%s About",
});
definePageMeta({
  layout: "app",
});
const technicalSkills = ref([
  { name: "HTML + CSS", i: "97" },
  { name: "Bootstrap", i: "97" },
  { name: "JavaScript", i: "97" },
  { name: "Vue.js", i: "93" },
  { name: "Vuex", i: "93" },
  { name: "Nuxt.js", i: "95" },
  { name: "Restful API/Axios", i: "96" },
]);
const personalSkills = ref([
  { name: "Self-Learning", i: "95" },
  { name: "Work for full time", i: "95" },
  { name: "Work with team", i: "95" },
  { name: "Adapt quickly", i: "95" },
  { name: "Knowledge of design rules", i: "95" },
  { name: "handle with fast situations", i: "95" },
  { name: "Learning and working under stress", i: "95" },
]);
</script>

<style></style>
