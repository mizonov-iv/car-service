<template>
  <button class="custom-btn rounded-pill p-2 px-4 fw-bold mt-2 d-block mx-auto font-medium">
    {{name}}
  </button>
</template>

<script>
export default {
  props: ["name"]
}
</script>

<style scoped>
.custom-btn {
  background-color: rgb(255, 234, 153);
  font-size: 18px;
}
</style>