<script>
import FooterBtn from "./FooterBtn.vue";
import FooterSocials from "./FooterSocials.vue";
export default {
  components: {
    FooterBtn,
    FooterSocials,
  },
};
</script>

<template>
  <div class="footer-bottom">
    <div class="container flex">
      <FooterBtn />
      <FooterSocials />
    </div>
  </div>
</template>

<style scoped lang="scss">
@use "../../styles/_partials/utilities.scss";
@use "../../styles/_partials/container.scss";
@use "../../styles/_partials/variables.scss" as *;

.footer-bottom {
  padding: 30px 0;
  background-color: $footer-bottom-bkg;
}
.container {
  justify-content: space-between;
  align-items: center;
}
</style>
