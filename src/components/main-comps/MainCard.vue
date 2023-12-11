<script>
export default {
  props: {
    url: String,
    title: String,
  },
};
</script>

<template>
  <div class="card">
    <div class="img-box">
      <img :src="url" :alt="title" />
    </div>
    <h4 class="upper">{{ title }}</h4>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/partials/variables" as *;
@use "../../assets/scss/partials/mixins" as *;
.card {
  @include grid($cards-per-row, $main-grid-gap);
  .img-box {
    aspect-ratio: 1 / 1;
    overflow: hidden;
  }
  h4 {
    padding: 20px 0;
    color: white;
    font-size: 12px;
    text-align: left;
  }
}
</style>
