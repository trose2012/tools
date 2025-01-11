<script setup lang="ts">
import { Toaster } from "@/components/ui/sonner";
const runtimeConfig = useRuntimeConfig();

useHead({
  link: [
    {
      rel: "icon",
      type: "image/svg+xml",
      href: "/favicon.ico",
    },
    {
      rel: "preconnect",
      href: "https://data.3kh0.net",
    },
  ],
  script: [
    {
      //todo add user consent
      src: "https://data.3kh0.net/script.js",
      "data-website-id": "3284c22d-b7ff-41dc-a622-f2d95899ee07",
      defer: true,
    },
  ],
  title: "Echo Net Extras", //todo add dynamic title
  // todo add meta tags
});
onMounted(() => {
  // timing
  const time = performance.now();
  window.addEventListener("load", () => {
    console.log(`Loaded in ${performance.now() - time}ms. Version ${runtimeConfig.public.sha}`);
  });
});
</script>

<template>
  <div id="app" class="bg-[#09090b] text-white flex flex-col md:flex-row overflow-hidden h-screen">
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
    <Toaster />
  </div>
</template>

<style>
/* fancy page transitions */
.page-enter-active,
.page-leave-active {
  transition: all 0.2s;
}
.page-enter-from,
.page-leave-to {
  opacity: 0;
  filter: blur(1rem);
}
</style>
