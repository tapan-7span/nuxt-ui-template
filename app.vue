<template>
  <div class="flex h-screen overflow-hidden">
    <sidebar />

    <div class="flex-1 flex flex-col">
      <div class="md:mx-10 m-4 md:my-4">
        <router-view></router-view>
      </div>
    </div>
  </div>
</template>
