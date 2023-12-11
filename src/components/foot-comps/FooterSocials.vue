<script>
export default {
  methods: {
    getImagePath: function (imgPath) {
      return new URL(imgPath, import.meta.url).href;
    },
  },
  data() {
    return {
      linkSocial: [
        {
          // img: "/src/assets/img/footer-facebook.png",
          img: "../../assets/img/footer-facebook.png",
          alt: "Facebook logo",
          href: "#",
        },
        {
          // img: "/src/assets/img/footer-twitter.png",
          img: "../../assets/img/footer-twitter.png",
          alt: "Twitter logo",
          href: "#",
        },
        {
          // img: "/src/assets/img/footer-youtube.png",
          img: "../../assets/img/footer-youtube.png",
          alt: "Yuotube logo",
          href: "#",
        },
        {
          // img: "/src/assets/img/footer-pinterest.png",
          img: "../../assets/img/footer-pinterest.png",
          alt: "Pinterest logo",
          href: "#",
        },
        {
          // img: "/src/assets/img/footer-periscope.png",
          img: "../../assets/img/footer-periscope.png",
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
          <img :src="getImagePath(social.img)" :alt="social.alt" />
        </a>
      </li>
    </ul>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/partials/variables" as *;

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
