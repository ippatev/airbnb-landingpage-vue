<template>
	<button class="icon-btn">
		<strong>
		Начать поиск
		</strong>
		<rounded-icon-button icon="search" class="icon"></rounded-icon-button>
	</button>
</template>

<script setup lang="ts">
import {RoundedIconButton} from "@/components"
</script>

<style lang="scss" scoped>
	.icon-btn {
		width: 300px;
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 8px 8px 8px 24px;
		background-color: #fff;
		border: 1px solid #DDDDDD !important;
		border-radius: 40px;
		box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.08), 0px 4px 12px rgba(0, 0, 0, 0.05) !important;

		&:hover {
			cursor: pointer;
			box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.08), 0px 6px 14px rgba(0, 0, 0, 0.05) !important;
		}
	}

</style>
