<!-- layouts/default.vue -->
<template>
  <NuxtLoadingIndicator />

  <v-layout>
    <!-- Page content -->
    <v-main>
      <v-container class="py-6" fluid>
        <slot />
      </v-container>
    </v-main>

    <v-footer class="px-4">
      <span class="text-caption">© {{ year }}</span>
    </v-footer>
  </v-layout>
</template>

<script setup lang="ts">
const year = new Date().getFullYear()
</script>
