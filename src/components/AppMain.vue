<script>
import MainJumbo from "./main-comps/MainJumbo.vue";
import MainContent from "./main-comps/MainContent.vue";
export default {
  components: {
    MainJumbo,
    MainContent,
  },
};
</script>

<template>
  <main>
    <MainJumbo />
    <MainContent />
  </main>
</template>

<style scoped lang="scss">
@use "../assets/scss/partials/variables" as *;
main {
  background-color: $main-bkg;
}
</style>
