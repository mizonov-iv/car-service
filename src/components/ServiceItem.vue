<template>
  <div class="col-11 col-md-5 text-light text-center" v-for="(item, index) in items" :key="index">
    <div class="fs-3 text-uppercase text-decoration-underline mt-3 font-bold">
      {{item.title}}
    </div>
    <div class="fs-5 mb-2 font-medium">
      {{item.subtitle}}
    </div>
    <div class="service-item___img">
      <img class="img-fluid" :src="`/img/${item.img}.jpg`" :alt="item.img">
    </div>
  </div>
</template>

<script>
export default {
props: ["items"]
}
</script>

<style scoped>
.service-item___img {
  border: 3px solid rgb(255, 234, 153);
}
</style>