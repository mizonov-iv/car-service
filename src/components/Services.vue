<template>
  <div class="services-wrapper">
    <div class="fs-2 fw-bold text-uppercase text-center text-light">
      <span style="color: rgb(255, 234, 153)">Любые виды услуг</span> <br> для вашего авто
    </div>
    <div class="px-md-5 d-flex flex-md-row justify-content-md-between">
      <ServiceItem :items="services"/>
    </div>
    <Button :name="'Проконсультироваться по телефону'"/>
    <div>
    </div>
  </div>
</template>

<script>
import ServiceItem from "./ServiceItem.vue";
import Button from "./Button.vue";
export default {
  components: {ServiceItem, Button},
data: () => ({
  services: [
    { title: "Диагностика", subtitle: "Компьютерная диагностика", img: "diagnostics" },
    { title: "Сервис", subtitle: "Техническое обслуживание", img: "service" },
    { title: "Ремонт", subtitle: "Любой сложности", img: "repair" },
  ],
})
}
</script>

<style scoped>
.services-wrapper {
  background-image: url("/img/services-gb.jpg");
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
}
</style>