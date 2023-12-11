<script>
export default {};
</script>

<template>
  <button>
    <a href="#" class="upper" target="_self">Sign-up now!</a>
  </button>
</template>

<style scoped lang="scss">
@use "../../assets/scss/partials/variables" as *;

button {
  background-color: transparent;
  height: 50px;
  border: 2px solid $primary-color;
  a {
    color: white;
    padding: 15px;
    font-weight: bold;
    font-size: 15px;
  }
}
</style>
