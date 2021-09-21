<template>
  <header class="app__header">
    <div class="app__header__item">
      <icon-logo></icon-logo>
    </div>
    <div class="app__header__item center">
      <icon-text-button></icon-text-button>
    </div>
    <div class="app__header__item">
      <div class="app__header__links">
        <router-link to="/about">Сдайте жилье</router-link>
        <rounded-icon-button icon="earth"></rounded-icon-button>
        <burger-button></burger-button>
      </div>
    </div>
  </header>
</template>

<script setup lang="ts">
import { IconTextButton, RoundedIconButton, BurgerButton } from "@/components";
import { IconLogo } from "@/components/icons";
</script>

<style lang="scss" scoped>
.app__header {
  width: 100%;
  display: flex;
  height: 80px;
  background-color: #fff;
  position: sticky;
  top: 0px;
  justify-content: space-between;
  align-items: center;
  box-shadow: rgba(0, 0, 0, 0.08) 0px 1px 12px !important;

  a {
    padding: 12px 10px;
    border-radius: 22px;
    font-size: 14px;
    font-weight: bold;
    color: #2c3e50;
    text-decoration: none;

    &.router-link-exact-active {
      color: #42b983;
    }

    &:hover {
      background-color: rgb(247, 247, 247);
    }
  }
}

.app__header__item {
  display: block;
  flex: 1 0 140px;

  &.center {
    flex: 0 1 auto;
  }
}

.app__header__links {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 8px;
}
</style>
