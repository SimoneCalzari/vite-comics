<script>
import HeaderLogo from "./head-comps/HeaderLogo.vue";
import HeaderMenu from "./head-comps/HeaderMenu.vue";
export default {
  components: {
    HeaderLogo,
    HeaderMenu,
  },
};
</script>

<template>
  <header>
    <div class="container flex">
      <HeaderLogo />
      <HeaderMenu />
    </div>
  </header>
</template>

<style scoped lang="scss">
@use "../styles/_partials/container.scss";
@use "../styles/_partials/utilities.scss";

.container {
  justify-content: space-between;
}
</style>
