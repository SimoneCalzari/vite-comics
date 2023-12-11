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
.container {
  justify-content: space-between;
}
</style>
