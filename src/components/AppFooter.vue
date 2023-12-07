<script>
import FooterTop from "./foot-comps/FooterTop.vue";
import FooterMid from "./foot-comps/FooterMid.vue";
import FooterBottom from "./foot-comps/FooterBottom.vue";
export default {
  components: {
    FooterTop,
    FooterMid,
    FooterBottom,
  },
};
</script>

<template>
  <footer>
    <FooterTop />
    <FooterMid />
    <FooterBottom />
  </footer>
</template>

<style scoped lang="scss"></style>
