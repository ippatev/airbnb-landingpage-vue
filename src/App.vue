<template>
	<app-header></app-header>
  <router-view/>
</template>

<script setup lang="ts">
import AppHeader from '@/components/AppHeader.vue';

</script>

<style lang="scss">
body {
	margin: 0;
}

#app {
	margin: 0 80px;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

</style>
