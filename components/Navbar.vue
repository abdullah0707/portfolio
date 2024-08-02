<template>
  <div class="navbar-action" :class="{ active: isActive }" @click="isActive = !isActive">
    <div class="menu-icon hover-target">
      <span class="menu-icon__line menu-icon__line-left"></span>
      <span class="menu-icon__line"></span>
      <span class="menu-icon__line menu-icon__line-right"></span>
    </div>
    <ul class="nav w-full flex items-center justify-center h-full">
      <li>
        <NuxtLink v-for="item in navigation" :key="item.name" @title="item.name" :to="item.href" :data-name="item.name"
          class="text-9xl md:text-8xl max-sm:text-4xl leading-loose topLeftBorders block">
          {{ item.name }}
        </NuxtLink>
      </li>
    </ul>
  </div>

  <div class="menu-nav"></div>
</template>

<script setup>
const isActive = ref(false);
const navigation = ref([
  { name: "HOME", href: "/" },
  { name: "About", href: "about" },
  { name: "Projects", href: "projects" },
  { name: "Contact", href: "contact" },
  { name: "Service", href: "service" },
]);
</script>
<style scoped>
ul li a {
  color: rgb(255, 255, 255);
  margin: 0.5em;
  transition: 0.3s;
}
ul li a:hover {
  cursor: pointer;
  margin-left: 0.6em;
}
</style>
