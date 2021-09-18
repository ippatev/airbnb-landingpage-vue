<template>
  <div class="card-img">
    <img class="card-img__image" :src="props.img" alt="Card image" />
    <strong class="card-img__title" v-text="props.title"></strong>
    <p class="card-img__subtitle" v-text="props.subtitle"></p>
  </div>
</template>

<script setup lang="ts">
const props = defineProps({
  img: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  subtitle: {
    type: String,
    required: false,
  },
});
</script>

<style lang="scss" scoped>
.card-img {
  display: flex;
  width: 100%;
  flex-direction: column;
  background-color: #fff;
  cursor: pointer;
}

.card-img > .card-img__image {
  border-radius: 8px;
  width: 100%;
  height: 100%;
}

.card-img > .card-img__title {
  margin-top: 8px;
  font-size: 18px;
  line-height: 22px;
}

.card-img > .card-img__subtitle {
  margin: 0;
  font-size: 14px;
}
</style>
