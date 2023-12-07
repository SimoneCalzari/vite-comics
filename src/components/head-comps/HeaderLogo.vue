<script>
export default {
  data() {
    return {
      logo: "/img/dc-logo.png",
      alt: "logo-pagina",
    };
  },
};
</script>

<template>
  <div>
    <img :src="logo" :alt="alt" />
  </div>
</template>

<style scoped lang="scss">
div {
  padding: 20px 0;
  width: 80px;
  flex-shrink: 0;
}
</style>
