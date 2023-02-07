<template>
  <div class="bg-dark">
    <div class="d-flex flex-column flex-md-row text-light px-2 px-md-4 p-3 mx-auto text-center justify-content-md-center align-items-baseline align-items-md-center">
      <a class="navbar-brand mx-auto d-md-none" href="#">
        <img src="/img/logo.png" alt="" style="width: 300px">
      </a>
      <div class="d-none d-md-block col fs-5 above-navbar-address">Ремонт автомобилей любой сложности</div>
      <div class="col d-flex mb-md-0 above-navbar-address">
        <svg xmlns="http://www.w3.org/2000/svg" width="26" height="26" fill="rgb(255, 234, 153)" class="bi bi-geo-alt-fill me-1" viewBox="0 0 16 16">
          <path d="M8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10zm0-7a3 3 0 1 1 0-6 3 3 0 0 1 0 6z"/>
        </svg>
        <div>Екатеринбург, ул. Раевского, д. 21, корп. А</div>
      </div>
      <div class="col d-flex above-navbar-address">
        <svg xmlns="http://www.w3.org/2000/svg" width="26" height="26" fill="rgb(255, 234, 153)" class="bi bi-gear-fill me-1" viewBox="0 0 16 16">
          <path d="M9.405 1.05c-.413-1.4-2.397-1.4-2.81 0l-.1.34a1.464 1.464 0 0 1-2.105.872l-.31-.17c-1.283-.698-2.686.705-1.987 1.987l.169.311c.446.82.023 1.841-.872 2.105l-.34.1c-1.4.413-1.4 2.397 0 2.81l.34.1a1.464 1.464 0 0 1 .872 2.105l-.17.31c-.698 1.283.705 2.686 1.987 1.987l.311-.169a1.464 1.464 0 0 1 2.105.872l.1.34c.413 1.4 2.397 1.4 2.81 0l.1-.34a1.464 1.464 0 0 1 2.105-.872l.31.17c1.283.698 2.686-.705 1.987-1.987l-.169-.311a1.464 1.464 0 0 1 .872-2.105l.34-.1c1.4-.413 1.4-2.397 0-2.81l-.34-.1a1.464 1.464 0 0 1-.872-2.105l.17-.31c.698-1.283-.705-2.686-1.987-1.987l-.311.169a1.464 1.464 0 0 1-2.105-.872l-.1-.34zM8 10.93a2.929 2.929 0 1 1 0-5.86 2.929 2.929 0 0 1 0 5.858z"/>
        </svg>
        <div>Ежедневно 10:00 - 19:00</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.above-navbar-img {
  display: block;
  margin: 0 auto;
  width: 65px;
  height: 50px;
}
.above-navbar-icons {
  width: 20px;
  margin-right: 8px;
}
.above-navbar-address {
  font-size: 16px;
  font-family: 'TT Norms';
  font-weight: bold;
  font-style: normal;
}
</style>