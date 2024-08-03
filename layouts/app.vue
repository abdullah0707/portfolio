<template>
   <div style="font-family: 'Allerta Stencil', sans-serif;">
      <Navbar />
      <div class="bg-text-container w-full overflow-hidden">
         <div class="animate-text">
            <span class="text-animate-bg">Front-End Developer&nbsp;</span>
            <span class="text-animate-bg">abdullah mohamed&nbsp;</span>
         </div>
         <div class="animate-text left">
            <span class="text-animate-bg">abdullah mohamed&nbsp;</span>
            <span class="text-animate-bg">Front-End Developer&nbsp;</span>
         </div>
         <div class="animate-text">
            <span class="text-animate-bg">Front-End Developer&nbsp;</span>
            <span class="text-animate-bg">abdullah mohamed&nbsp;</span>
         </div>
      </div>
      <div class="_social-links">
         <ul class="_links-list">
            <li class="_social-link">
               <NuxtLink to="https://www.facebook.com/abdullah.mohammed93" target="_blank"><i
                     class="fa-brands fa-square-facebook"></i></NuxtLink>
            </li>
            <li class="_social-link">
               <NuxtLink to="https://www.linkedin.com/in/abdullah-mohammed-b47234121/" target="_blank"><i
                     class="fa-brands fa-linkedin"></i></NuxtLink>
            </li>
            <li class="_social-link">
               <NuxtLink to="https://github.com/abdullah0707" target="_blank"><i class="fa-brands fa-square-git"></i>
               </NuxtLink>
            </li>
            <!-- <li class="_social-link"><a  href="mailto:abdullahelgammal25@gmail.com" target="_blank"><i class="fa-solid fa-envelope"></i></a></li> -->
            <li class="_social-link">
               <NuxtLink to="https://wa.me/qr/ZPSAINJL44YEP1" target="_blank"><i
                     class="fa-brands fa-square-whatsapp"></i></NuxtLink>
            </li>
            <li class="_social-link">
               <NuxtLink to="tel:+201094242767"><i class="fa-solid fa-square-phone"></i></NuxtLink>
            </li>
         </ul>
      </div>
      <slot />
   </div>
</template>

<script setup>

</script>
<style></style>