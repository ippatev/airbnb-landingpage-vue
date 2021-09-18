<template>
	<span class="rounded-icon-btn">
		<keep-alive>
			<component :is="IconComponent"></component>
		</keep-alive>
	</span>	
</template>

<script setup lang="ts">
import { computed, ref } from "vue"
import { IconSearch } from "@/components/icons"
import { IconEarth } from "@/components/icons"

const color = ref("#fff");

const props = defineProps({
	icon: {
		type: String,
		required: true
	}
})

const IconComponent = computed(() => {
	switch(props.icon) {
		case "search":
			color.value = "#FF5A5F"
			return IconSearch;
		case "earth":
			return IconEarth;
	}
})

</script>

<style lang="scss" scoped>
.rounded-icon-btn {
	display: flex;
	justify-content: center;
	align-items: center;
	width: 32px;
	height: 32px;
	border-radius: 50%;
	background-color: v-bind(color);
	cursor: pointer;
}

</style>
