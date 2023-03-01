<template>
  <div class="services-wrapper" id="about">
    <div class="fs-2 fw-bold text-uppercase text-center text-light font-bold">
      <span style="color: rgb(255, 234, 153)">Любые виды услуг</span> <br> для вашего авто
    </div>
    <div class="px-md-5 d-flex flex-column align-items-center flex-md-row justify-content-md-between mb-4">
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
    { title: "Малярные работы", subtitle: "Строгое следование технологии кузовного ремонта и малярных работ, не зависимо от объема ремонта кузова", img: "painting" },
    { title: "Покраска", subtitle: "Только современное оборудование и квалифицированные специалисты", img: "painting2" },
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
  padding: 10px 0px 10px 0px;
}
</style>