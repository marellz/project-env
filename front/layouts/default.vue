<template>
  <div class="flex flex-col h-[100vh] bg-gray-100">
    <app-header />
    <main class="flex-auto">
      <slot />
    </main>
    <app-footer />
  </div>
</template>
