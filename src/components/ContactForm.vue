<template>
  <div class="p-md-4">
    <div class="d-none d-md-block mx-auto rounded contact-form">
      <h2  class="text-center contact-form__header">ЗАПИШИТЕСЬ НА БЕСПЛАТНУЮ ДИАГНОСТИКУ ВАШЕГО АВТО</h2>
      <p class="text-light text-center">Заполните форму ниже, приезжайте к нам и получите реальную ситуацию по Вашему автомобилю</p>
      <form class="needs-validation" novalidate>
        <div class="mb-3 form-floating has-validation">
          <input
              type="text"
              class="form-control rounded-pill contact-form__border"
              placeholder="Введите имя"
              v-model="form.name"
              id="validationUsername"
              required
          >
          <label for="validationUsername">Ваше имя</label>
          <div class="invalid-feedback">
            Введите имя
          </div>
        </div>
        <div class="mb-3 form-floating has-validation">
          <input
              type="tel"
              class="form-control rounded-pill contact-form__border"
              placeholder="+7 999-999-99-99"
              v-model="form.phone"
              v-mask="'+7(###)###-##-##'"
              id="validationPhone"
              required
          >
          <label for="validationPhone">Номер телефона</label>
          <div class="invalid-feedback">
            Введите номер телефона
          </div>
        </div>
        <button
            type="submit"
            class="btn w-100 rounded-pill p-3 contact-form__btn"
            data-bs-toggle="modal"
            data-bs-target="#exampleModal"
            @click.prevent="sendMessage"
            :disabled="this.form.name === '' || this.form.phone === ''"
        >
          Записаться на диагностику
        </button>
      </form>
    </div>
<!--    <SuccessPopUp id="exampleModal" aria-labelledby="exampleModalLabel" aria-hidden="true"/>-->
  </div>

</template>

<script>
// import {mask} from "vue-the-mask";
import axios from "axios";
import {mask} from "vue-the-mask"

export default {
  data: () => ({
    form: {
      name: "",
      phone: ""
    },
  }),
  directives: {mask},
  methods: {
    sendMessage() {

      const TOKEN = "5688324213:AAENCPbMFOKejLYK-SN-tITi5io1I6sQJ2I"
      const CHAT_ID = "-1001506049425"
      const URI_API = `https://api.telegram.org/bot${ TOKEN }/sendMessage`

      let message = `<b>Заявка с сайта</b>\n`
      message += `<b>Отправитель: </b> ${this.form.name} \n`
      message += `<b>Телефон: </b> ${this.form.phone}`

      axios.post(URI_API, {
        chat_id: CHAT_ID,
        parse_mode: 'html',
        text: message
      })

      this.form.name = ""
      this.form.phone = ""
    }
  }
}
</script>

<style scoped>
.contact-form {
  border: 3px solid rgb(255, 234, 153);
  padding: 15px 15px;
}
.contact-form__header {
  font-size: 22px;
  color: rgb(255, 234, 153);
}
.contact-form__border {
  border: 5px solid rgb(255, 234, 153);
}
.contact-form__btn {
  background-color: rgb(255, 234, 153);
}
</style>