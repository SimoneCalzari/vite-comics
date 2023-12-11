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
@use "../../assets/scss/partials/variables" as *;

.footer-bottom {
  padding: 30px 0;
  background-color: $footer-bottom-bkg;
}
.container {
  justify-content: space-between;
  align-items: center;
}
</style>
