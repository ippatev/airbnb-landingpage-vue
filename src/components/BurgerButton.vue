<template>
	<button class="btn-burger">
		<icon-burger></icon-burger>	
		<img src="@/assets/avatar.png" alt="User avatar">
	</button>	
</template>

<script setup lang="ts">
import { IconBurger } from "@/components/icons"
</script>

<style lang="scss" scoped>
.btn-burger {
	display: flex;
	background-color: #fff;
	border: 1px solid #DDDDDD;
	justify-content: center;
	align-items: center;
	padding: 4px 4px 4px 16px;
	border-radius: 20px;
	outline: none;
	cursor: pointer;
	gap: 8px;
}
</style>
