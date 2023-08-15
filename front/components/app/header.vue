<template>
  <header>
    <layout-container class="py-10">
        <div class="flex justify-center">
            <ul class="flex">
              <li v-for="(link, index) in links" :key="index">
                <nuxt-link :to="link.path" class="block px-4 py-2 bg-gray-50"> {{ link.label }}</nuxt-link>
              </li>
            </ul>
        </div>
    </layout-container>
  </header>
</template>
<script lang="ts" setup>
const links = [
    { label: "home", path: "/" },
    { label: "about", path: "/about" },
    { label: "faq", path: "/faq" },
    ];
</script>
