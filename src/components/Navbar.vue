<template>
  <nav class="navbar navbar-expand-lg navbar-dark px-3" style="background-color: #101112">
    <div class="container-fluid" id="main">
      <a class="navbar-brand d-none d-md-block" href="#main">
        <img src="/img/logo.png" alt="" style="width: 300px">
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0 fs-5">
          <li class="nav-item item-hover">
            <a class="nav-link " href="#main">Главная</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#about">О сервисе</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#contact">Спецпредложения</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#contacts">Контакты</a>
          </li>
        </ul>
        <div class="d-flex flex-column mx-auto text-light">
          <a class="text-center text-decoration-underline text-light fs-4" style="cursor: pointer"  href="tel:+79221352345">+7-922-135-23-45</a>
          <a class="d-block custom-btn rounded-pill p-2 px-4 fw-bold mt-2 d-block mx-auto font-medium text-decoration-none text-dark" href="#contact">
            Заказать звонок
          </a>
        </div>
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
.item-hover:hover{
  color: red;
}

.custom-btn {
  background-color: rgb(255, 234, 153);
  font-size: 18px;
  cursor: pointer;
}
</style>