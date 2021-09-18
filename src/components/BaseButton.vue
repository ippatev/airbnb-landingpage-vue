<template>
  <button class="base-btn">
    <slot></slot>
  </button>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.base-btn {
  background-color: #fff;
  border-radius: 8px;
  color: #000;
  padding: 16px 24px;
  font-weight: bold;
  font-size: 18px;
  border: none;
  outline: none;
  cursor: pointer;
}
</style>
