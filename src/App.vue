<template>
  <app-header></app-header>
  <main class="container">
    <router-view />
  </main>
  <app-footer></app-footer>
</template>

<script setup lang="ts">
import { AppHeader, AppFooter } from "@/components";
</script>

<style lang="scss">
*,
*::after,
*::before {
  box-sizing: border-box;
}

body {
  margin: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

#app > header,
main,
footer {
  padding: 0 80px;
}

.container {
  margin-top: 32px;
}
</style>
