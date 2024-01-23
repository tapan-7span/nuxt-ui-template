import type { NuxtLink } from '#build/components';
<template>
  <div class="flex flex-col space-y-2">
    <NuxtLink
      v-for="route in sortedRoutes"
      :key="route.name"
      :to="route.path"
      class="w-full p-2 border rounded-md bg-neutral-900 hover:bg-neutral-800 transition-all duration-300 capitalize border-neutral-600"
    >
      {{ route.name }}
    </NuxtLink>
  </div>
</template>

<script setup>
const router = useRouter();
const all_routes = router.options.routes;
const sortedRoutes = all_routes.sort((a, b) => a.name.localeCompare(b.name));

// TODO :  If there is any kind of record
</script>
<style>
.router-link-active {
  @apply bg-neutral-800 border-neutral-500;
}
</style>
