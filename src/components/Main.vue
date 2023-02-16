<template>
  <div>
    <div class="text-center fw-bold fs-2 py-2 slogan">
      Несем личную ответственность за каждый автомобиль!
    </div>
    <div class="main">
      <div class="text-light text-center fw-bold fs-1 pt-4 px-1 px-md-5 font-bold text-uppercase">
        Автосервис по ремонту и обслуживанию <br> автомобилей всех марок
      </div>
      <div class="d-flex flex-column flex-md-row justify-content-md-between align-items-md-center p-md-2 px-md-5">
        <ContactForm class="mx-auto col-11 col-md-5"/>
        <div class="mx-auto mt-3 col-11 col-md-7 fs-5 text-md-start text-center text-light font-regular">
          Автосервис в Екатеринбурге предоставляет разный спектр услуг по обслуживанию всех марок авто отечественного и зарубежного производства.
          Мы про качество. <br>
          Автосервис г. Екатеринбург "VService" <br>
          Ремонт автомобилей любой сложности, в частности: ремонт ДВС, МКПП, замена масла в АКПП, покраска, полировка.
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
  font-family: 'TT Norms';
  font-weight: bold;
  font-style: normal;
  letter-spacing: 0.5px;
}
.main {
  height: 100%;
  background-image: url("/img/bg.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
</style>