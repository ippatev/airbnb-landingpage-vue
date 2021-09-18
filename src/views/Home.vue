<template>
  <div class="home-page"> 
		<header>
			Живите где угодно
		</header>

		<ul class="img-cards">
			<li v-for="card in imageCards" :key="card.title">
				<image-card :title="card.title" :img="card.imageUrl"/>
			</li>
		</ul>
  </div>
</template>

<script setup lang="ts">
import { ImageCard } from "@/components";
import { IImageCard } from "@/models/ImageCard"

const imageCards: IImageCard[] = [
	{
		title: "Жилье на природе",
		imageUrl: "https://a0.muscache.com/im/pictures/2f13349d-879d-43c6-83e3-8e5679291d53.jpg?im_w=720"
	},
	{
		title: "Уникальное жилье",
		imageUrl: "https://a0.muscache.com/im/pictures/36f53e61-db8d-403c-9122-5b761c0e4264.jpg?im_w=720"
	},
	{
		title: "Жилье целиком",
		imageUrl: "https://a0.muscache.com/im/pictures/7d82ca14-56e5-4465-8218-dcfa7d69b6ac.jpg?im_w=720"
	},
	{
		title: "Можно с животными",
		imageUrl: "https://a0.muscache.com/im/pictures/10a638e1-6aff-4313-8033-1275cec83987.jpg?im_w=720"
	},
]

</script>

<style lang="scss" scoped>
.home-page {
}

.home-page > header {
	font-weight: bold;
	font-size: 32px;
}

.img-cards {
	display: flex;
	gap: 16px;
	margin: 0;
	margin-top: 32px;
	padding: 0;
	list-style: none;
}

</style>
