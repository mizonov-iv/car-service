<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark" style="background-color: #00060a">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Логотип</a>

      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item dropdown">
            <a class="nav-link active dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              Услуги
            </a>
            <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
              <li><a class="dropdown-item" href="#">Диагностика автомобиля</a></li>
              <li><a class="dropdown-item" href="#">Ремонт двигателя</a></li>
              <li><a class="dropdown-item" href="#">Ремонт трансмиссии</a></li>
              <li><a class="dropdown-item" href="#">Ремонт подвески</a></li>
              <li><a class="dropdown-item" href="#">Ремонт тормозной системы</a></li>
              <li><a class="dropdown-item" href="#">Комьютерная диагностика</a></li>
              <li><a class="dropdown-item" href="#">Шиномонтаж</a></li>
            </ul>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">О компании</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Контакты</a>
          </li>
        </ul>
        <a class="navbar-brand" href="#">
          <img src="/icons/telegram-icon.svg" alt="">
        </a>
        <a class="navbar-brand" href="#">
          <img src="/icons/whatsapp-icon.svg" alt="">
        </a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {

}
</script>

<style scoped>
.navbar-toggler-icon {
  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba(231, 205, 108, 1), 0, 0, 0.55%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");
}
.navbar-toggler {
  border: none;
}
</style>