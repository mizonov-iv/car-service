<template>
  <button
      class="custom-btn rounded-pill p-2 px-4 fs-5
      fw-bold
      m-4
      d-block
      mx-auto
"
  >
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
}
</style>