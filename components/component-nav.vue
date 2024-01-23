<template>
  <!-- <div class="flex flex-col">
      {{ componentNames }}
    </div> -->
</template>

<script setup>
import { ref } from 'vue';
// import { import.meta } from 'vue-meta';
const componentNames = ref([]);

// (async () => {
//   const modules = await import.meta.glob('@/components/*');
//   componentNames.value = Object.keys(modules).map((path) => path.replace('@/components/', ''));
// })();
</script>
