<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark" style="background-color: #00060a">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Логотип</a>

      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item item-hover">
            <a class="nav-link " href="#">
              Главная
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">О сервисе</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Спецпредложения</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Отзывы</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Контакты</a>
          </li>
        </ul>
        <div class="d-flex text-light">
          <div>
            <img src="/icons/Untitled.svg" alt="">
          </div>
          <div class="d-flex flex-column">
            <div>
              +7-922-135-23-45
            </div>
            <div>
              <button>Заказать звонок</button>
            </div>
          </div>

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
</style>