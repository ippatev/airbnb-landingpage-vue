<template>
	<div class="big-card">
		<div class="big-card__content">
			<div class="big-card__title">
				Принимать гостей
			</div>
			<div class="big-card__subtitle">
				Открывайте новые возможности и получайте доход, сдавая жилье.
			</div>
		</div>
		<div class="big-card__actions">
			<base-button>
				Подробнее
			</base-button>	
		</div>
	</div>	
</template>

<script setup lang="ts">
	import BaseButton from "@/components/BaseButton.vue";
</script>

<style lang="scss" scoped>
.big-card	{
	display: flex;
	flex-direction: column;
	justify-content: center;
	width: auto;
	height: 480px;
	background-image: url("https://a0.muscache.com/im/pictures/2595054e-d1d9-4fde-8046-58d51fcb3164.jpg?im_w=1440");
	background-size: cover;
	background-repeat: no-repeat;
	border-radius: 16px;
	padding: 0 80px;
}

.big-card > .big-card__content {
	width: 360px;
	color: #fff;
}

.big-card__title {
	font-weight: bold;
	font-size: 48px;
}

.big-card__subtitle {
	margin-top: 16px;
	font-size: 18px;
	line-height: 24px;
}

.big-card > .big-card__actions {
	margin-top: 40px;
}
</style>
