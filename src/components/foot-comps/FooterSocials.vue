<script>
export default {
  data() {
    return {
      linkSocial: [
        {
          img: "/img/footer-facebook.png",
          alt: "Facebook logo",
          href: "#",
        },
        {
          img: "/img/footer-twitter.png",
          alt: "Twitter logo",
          href: "#",
        },
        {
          img: "/img/footer-youtube.png",
          alt: "Yuotube logo",
          href: "#",
        },
        {
          img: "/img/footer-pinterest.png",
          alt: "Pinterest logo",
          href: "#",
        },
        {
          img: "/img/footer-periscope.png",
          alt: "Periscope logo",
          href: "#",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="socials flex">
    <h3 class="upper">Follow us</h3>
    <ul class="flex">
      <li v-for="social in linkSocial">
        <a :href="social.href">
          <img :src="social.img" :alt="social.alt" />
        </a>
      </li>
    </ul>
  </div>
</template>

<style scoped lang="scss">
@use "../../styles/_partials/utilities.scss";
@use "../../styles/_partials/variables.scss" as *;

.socials {
  align-items: center;
}

h3 {
  color: $primary-color;
  margin-right: 25px;
}

ul {
  gap: 15px;
  li {
    border-radius: 50%;
    overflow: hidden;
  }
}
</style>
