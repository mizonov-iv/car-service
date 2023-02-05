<template>
  <div>
    <div class="text-center fw-bold fs-2 py-2 slogan">
      Несем личную ответственность за каждый автомобиль!
    </div>
    <div class="main">
      <div class="text-light text-center fw-bold fs-1 pt-4 px-5">
        Автосервис по ремонту и обслуживанию <br> автомобилей всех марок
      </div>
      <div class="d-flex p-2 mx-auto">
        <ContactForm class="col-md-5"/>
        <div class="col-md-5 fs-5 text-light">
          Автосервис в Екатеринбурге предоставляет разный спектр услуг по обслуживанию всех марок авто отечественного и зарубежного производства.
          Мы про качество. <br>
          Автосервис г. Екатеринбург "VService" <br>
          Ремонт автомобилей любой сложности, в частности: ремонт ДВС, МКПП, замена масла в АКПП, покраска, полировка.
          <br>
          Производим диагностику сход-развала и подготовку к техосмотру. <br>
          Также осуществляем работы по шиномонтажу, диагностике шин.
        </div>
      </div>
      <div>
        Иконки услуг
      </div>
    </div>
  </div>
</template>

<script>
import ContactForm from "./ContactForm.vue";
export default {
  components: {ContactForm}
}
</script>

<style scoped>
.slogan {
  background-color: rgb(255, 234, 153);
  color: #262626;
}
.main {
  height: 100%;
  background-image: url("/img/bg.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
</style>