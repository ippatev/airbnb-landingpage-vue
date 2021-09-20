<template>
  <footer>
    <div class="row">
      <div class="col" v-for="col of cols" :key="col.title">
        <header v-text="col.title"></header>
        <span v-for="link of col.links" :key="link" v-text="link"> </span>
      </div>
    </div>
  </footer>
</template>

<script setup lang="ts">
const cols = [
  {
    title: "О НАС",
    links: [
      "Как устроена платформа Airbnb",
      "Пресс-центр",
      "Airbnb 2021",
      "Для инвесторов",
      "Airbnb Plus",
      "Airbnb Luxe",
      "HotelTonight",
      "Airbnb для бизнеса",
      "С хозяевами возможно всё",
      "Карьера в Airbnb",
      "Письмо от основателей Airbnb",
    ],
  },
  {
    title: "СООБЩЕСТВО",
    links: [
      "Личностное многообразие и принятие",
      "Доступность",
      "Принимайте афганских беженцев",
      "Гости-рефералы",
      "Airbnb.org",
    ],
  },
  {
    title: "ПРИНИМАЙТЕ ГОСТЕЙ",
    links: [
      "Сдайте жилье",
      "Организуйте онлайн-Впечатление",
      "Организуйте Впечатление",
      "Ответственный прием гостей",
      "Центр ресурсов",
      "Центр общения",
    ],
  },
  {
    title: "ПОДДЕРЖКА",
    links: [
      "Действия Airbnb во время пандемии",
      "Центр помощи",
      "Отмена в период пандемии",
      "Поддержка соседей",
      "Доверие и безопасность",
    ],
  },
];
</script>

<style lang="scss" scoped>
footer {
  border-top: 1px solid #dddddd;
  background-color: #f7f7f7;
}

.row {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: top;
  padding: 80px 80px 80px 0px;
}

.col {
  display: flex;
  flex-direction: column;
}

.col > header {
  font-weight: bold;
  font-size: 12px;
}

.col > span {
  margin-top: 16px;
  font-size: 14px;
  font-weight: 100;
}
</style>
