<template>
   <div class="custom-section h-dvh overflow-scroll">
      <h1 class="text-center font-semibold text-white text-7xl py-3.5">
         Service
      </h1>
      <div class="grid grid-flow-row-dense md:grid-cols-2 grid-cols-1">
         <UCard class="m-4 bg-slate-400">
            <h5 class="text-amber-400">
               UX Research
            </h5>
            <p class="text-zinc-300">
               It’s important to research deeply for the product you want to build. We help in that by defining the
               user audience, working on user stories, competitive analysis and much more.
            </p>
         </UCard>
         <UCard class="m-4 bg-slate-400">
            <h5 class="text-amber-400">
               UX Auditing
            </h5>
            <p class="text-zinc-300">
               If you are unsure of how your app behaves, we can help by doing a detailed UX audit that will highlight
               most of the issues in your product. From there, we can take it further and fix all issues.
            </p>
         </UCard>
      </div>

      <div class="grid grid-flow-row-dense md:grid-cols-5 grid-cols-1">
         <UCard class="m-4 col-span-2 card">
            <h5 class="text-amber-400">
               UX Consultation
            </h5>
            <p class="text-zinc-300">
               If you don’t know what kind of service to request from us, don’t worry. We can help and see what fits
               your business and your budget.
            </p>
         </UCard>
         <UCard class="m-4 col-span-3">
            <h5 class="text-amber-400">
               Front End Development
            </h5>
            <p class="text-zinc-300">
               We are Front End masters with a deep focus on HTML, CSS, JavaScript The result of our work is a
               responsive,
               accessible, and performant websites. Either you have the design ready and want us to code it, or you want
               us to do both design and code, we’re happy to do so.
            </p>
         </UCard>
      </div>
      <div class="grid grid-flow-row-dense md:grid-cols-5 grid-cols-1">
         <UCard class="m-4 col-span-3">
            <h5 class="text-amber-400">
               Mobile Apps Design
            </h5>
            <p class="text-zinc-300">
               To reach more customers and the goals of your business, a mobile application is necessary these days. We
               will work on the app design from scratch to final tested prototype.
            </p>
         </UCard>
         <UCard class="m-4 col-span-2">
            <h5 class="text-amber-400">
               Responsive Web Design
            </h5>
            <p class="text-zinc-300">
               We leverage the concept of mobile-first design. Through our work, we focus on designing an experience
               that works across different screen sizes.
            </p>
         </UCard>
      </div>
   </div>
</template>

<script setup>

useHead({
   titleTemplate: "%s Service",
});

   definePageMeta({
      layout: 'app'
   })

</script>

<style>

</style>