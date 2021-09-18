<template>
  <div class="app__header">
		<div class="app__header__item">
			<icon-logo></icon-logo>
		</div>
		<div class="app__header__item">
			<icon-button></icon-button>
		</div>
		<div class="app__header__item">
			<router-link to="/about">Сдайте жилье</router-link>
			<rounded-icon-button icon="earth"></rounded-icon-button>
		</div>
  </div>
</template>

<script setup lang="ts">
import { IconButton, RoundedIconButton } from "@/components"
import { IconLogo } from "@/components/icons"

</script>

<style lang="scss" scoped>
.app__header {
	display: flex;
	height: 80px;
	justify-content: space-between;
	align-items: center;

  a {
    font-weight: bold;
    color: #2c3e50;
		text-decoration: none;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

.app__header__item {
	display: flex;
	align-items: center;
	gap: 8px
}
</style>
