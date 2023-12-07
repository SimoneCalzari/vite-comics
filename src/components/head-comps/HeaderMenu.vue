<script>
export default {
  data() {
    return {
      links: [
        {
          title: "Characters",
          href: "#",
          target: "_self",
        },
        {
          title: "Comics",
          href: "#",
          target: "_self",
        },
        {
          title: "Movies",
          href: "#",
          target: "_self",
        },
        {
          title: "Tv",
          href: "#",
          target: "_self",
        },
        {
          title: "Games",
          href: "#",
          target: "_self",
        },
        {
          title: "Collectibles",
          href: "#",
          target: "_self",
        },
        {
          title: "Videos",
          href: "#",
          target: "_self",
        },
        {
          title: "Fans",
          href: "#",
          target: "_self",
        },
        {
          title: "News",
          href: "#",
          target: "_self",
        },
        {
          title: "Shop",
          href: "#",
          target: "_self",
        },
      ],
    };
  },
};
</script>

<template>
  <ul class="flex">
    <li v-for="link in links" class="upper">
      <a :href="link.href" :target="link.target">{{ link.title }}</a>
    </li>
  </ul>
</template>

<style scoped lang="scss">
@use "../../styles/_partials/utilities.scss";
@use "../../styles/_partials/variables.scss" as *;

ul {
  gap: 30px;
  a {
    line-height: 115px;
    font-size: 12px;
    color: black;
    display: block;
    height: 100%;
    font-weight: bold;
    &:hover {
      color: $primary-color;
      border-bottom: 5px solid $primary-color;
    }
  }
}
</style>
