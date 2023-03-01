<template>
  <footer class="footer mt-auto p-3 text-light footer-wrapper">
    <div class="container d-flex flex-column justify-content-center align-items-center flex-md-row justify-content-md-between">
      <div class="col-11 col-md-6">
        <div id="map" style="width: 100%; height: 400px"></div>
      </div>
      <div class="col-11 col-md-6 px-3">
        <div class="fs-3 fw-bold font-bold mt-md-0 mt-4" id="contacts">Контакты</div>
        <div class="d-flex mt-3">
          <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" fill="rgb(255, 234, 153)" class="bi bi-geo-alt-fill me-2" viewBox="0 0 16 16">
            <path d="M8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10zm0-7a3 3 0 1 1 0-6 3 3 0 0 1 0 6z"/>
          </svg>
          <p class="fs-5 fw-bold font-medium">Екатеринбург, <br class="d-md-none"> ул. Раевского, <br class="d-md-none">д. 21, корп. А</p>
        </div>
        <div class="d-flex mt-3">
          <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" fill="rgb(255, 234, 153)" class="bi bi-telephone-fill me-2" viewBox="0 0 16 16">
            <path fill-rule="evenodd" d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511z"/>
          </svg>
          <a class="fs-5 fw-bold font-medium text-light text-decoration-none" href="tel:+79221352345">+7-922-135-23-45</a>
        </div>
        <div class="d-flex mt-3">
          <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" fill="rgb(255, 234, 153)" class="bi bi-telegram me-2" viewBox="0 0 16 16">
            <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zM8.287 5.906c-.778.324-2.334.994-4.666 2.01-.378.15-.577.298-.595.442-.03.243.275.339.69.47l.175.055c.408.133.958.288 1.243.294.26.006.549-.1.868-.32 2.179-1.471 3.304-2.214 3.374-2.23.05-.012.12-.026.166.016.047.041.042.12.037.141-.03.129-1.227 1.241-1.846 1.817-.193.18-.33.307-.358.336a8.154 8.154 0 0 1-.188.186c-.38.366-.664.64.015 1.088.327.216.589.393.85.571.284.194.568.387.936.629.093.06.183.125.27.187.331.236.63.448.997.414.214-.02.435-.22.547-.82.265-1.417.786-4.486.906-5.751a1.426 1.426 0 0 0-.013-.315.337.337 0 0 0-.114-.217.526.526 0 0 0-.31-.093c-.3.005-.763.166-2.984 1.09z"/>
          </svg>
          <a class="fs-5 fw-bold font-medium text-light text-decoration-none" href="https://t.me/vservice96" style="cursor: pointer">@vservice96</a>
        </div>
      </div>
    </div>
    <div class="d-flex flex-column flex-md-row justify-content-md-between align-items-center">
      <div class="fs-5 col-md-3 font-medium text-center mt-md-0 mt-3">Ремонт, обслуживание и диагностика в г. Екатеринбурге</div>
      <div class="col-md-3 mt-2">
        <img src="/img/logo.png" alt="" style="width: 300px">
      </div>
      <div class="d-flex flex-column col-md-3">
        <p class="text-center font-medium mt-2">Остались вопросы? Задайте их специалисту</p>
        <a class="d-block custom-btn rounded-pill p-2 px-4 fw-bold mt-2 d-block mx-auto font-medium text-decoration-none text-dark" href="tel:+79221352345">
          Обратиться
        </a>
      </div>
    </div>
    <p class="text-center">© 2022, «VService», г. Екатеринбург. Все права защищены.</p>
  </footer>
</template>

<script>
export default {
  created() {
    let center = [56.854153, 60.669394];

    function init() {
      let map = new ymaps.Map('map', {
        center: center,
        zoom: 15
      });

      map.controls.remove('geolocationControl'); // удаляем геолокацию
      map.controls.remove('searchControl'); // удаляем поиск
      map.controls.remove('trafficControl'); // удаляем контроль трафика
      map.controls.remove('typeSelector'); // удаляем тип
      map.controls.remove('fullscreenControl'); // удаляем кнопку перехода в полноэкранный режим
      map.controls.remove('zoomControl'); // удаляем контрол зуммирования
      map.controls.remove('rulerControl'); // удаляем контрол правил
      map.behaviors.disable(['scrollZoom']); // отключаем скролл карты (опционально)
      map.geoObjects.add(new ymaps.Placemark([56.854153, 60.669394], {
        iconCaption: "VService",
        iconLayout: 'default#image',
        iconImageHref: 'https://image.flaticon.com/icons/png/512/64/64113.png',
        iconImageSize: [40, 40],
        iconImageOffset: [-19, -44]
      }))
    }

    ymaps.ready(init);
  }
}
</script>

<style scoped>
.footer-wrapper {
  background-color: #101112;
}

.custom-btn {
  background-color: rgb(255, 234, 153);
  font-size: 18px;
  cursor: pointer;
}
</style>