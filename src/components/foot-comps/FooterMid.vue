<script>
export default {
  data() {
    return {
      shopList: [
        {
          text: "Shop DC",
          href: "#",
          target: "_self",
        },
        {
          text: "Shop DC Collectibles",
          href: "#",
          target: "_self",
        },
      ],
      sitesList: [
        {
          text: "DC",
          href: "#",
          target: "_self",
        },
        {
          text: "MAD Magazine",
          href: "#",
          target: "_self",
        },
        {
          text: "DC Kids",
          href: "#",
          target: "_self",
        },
        {
          text: "DC Universe",
          href: "#",
          target: "_self",
        },
        {
          text: "DC Power Visa",
          href: "#",
          target: "_self",
        },
      ],
      dcComicsList: [
        {
          text: "Characters",
          href: "#",
          target: "_self",
        },
        {
          text: "Comics",
          href: "#",
          target: "_self",
        },
        {
          text: "Movies",
          href: "#",
          target: "_self",
        },
        {
          text: "TV",
          href: "#",
          target: "_self",
        },
        {
          text: "Games",
          href: "#",
          target: "_self",
        },
        {
          text: "Videos",
          href: "#",
          target: "_self",
        },
        {
          text: "News",
          href: "#",
          target: "_self",
        },
      ],
      dcList: [
        {
          text: "Terms Of Use",
          href: "#",
          target: "_self",
        },
        {
          text: "Privacy policy(News)",
          href: "#",
          target: "_self",
        },
        {
          text: "Ad Choices",
          href: "#",
          target: "_self",
        },
        {
          text: "Advertising",
          href: "#",
          target: "_self",
        },
        {
          text: "Jobs",
          href: "#",
          target: "_self",
        },
        {
          text: "Subscriptions",
          href: "#",
          target: "_self",
        },
        {
          text: "Talent Workshops",
          href: "#",
          target: "_self",
        },
        {
          text: "CPSC Certificates",
          href: "#",
          target: "_self",
        },
        {
          text: "Ratings",
          href: "#",
          target: "_self",
        },
        {
          text: "Shop Helps",
          href: "#",
          target: "_self",
        },
        {
          text: "Contact Us",
          href: "#",
          target: "_self",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="footer-mid">
    <div class="container flex">
      <!-- COL 1 -->
      <div class="col">
        <!-- DC COMICS -->
        <h3 class="upper">dc comics</h3>
        <ul>
          <li v-for="li in dcComicsList">
            <a :href="li.href" :target="li.target">{{ li.text }}</a>
          </li>
        </ul>
        <!-- /DC COMICS -->
        <!-- SHOP -->
        <h3 class="upper">shop</h3>
        <ul>
          <li v-for="li in shopList">
            <a :href="li.href" :target="li.target">{{ li.text }}</a>
          </li>
        </ul>
        <!-- /SHOP -->
      </div>
      <!-- /COL 1 -->
      <!-- COL 2 -->
      <div class="col">
        <!-- DC -->
        <h3 class="upper">dc</h3>
        <ul>
          <li v-for="li in dcList">
            <a :href="li.href" :target="li.target">{{ li.text }}</a>
          </li>
        </ul>
        <!-- /DC -->
      </div>
      <!-- /COL 2 -->
      <!-- COL 3 -->
      <div class="col">
        <!-- SITES -->
        <h3 class="upper">sites</h3>
        <ul>
          <li v-for="li in sitesList">
            <a :href="li.href" :target="li.target">{{ li.text }}</a>
          </li>
        </ul>
        <!-- /SITES -->
      </div>
      <!-- /COL 3 -->
    </div>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/css/_partials/variables" as *;

.footer-mid {
  background-image: url("../../assets/img/footer-bg.jpg");
}

.container {
  padding-top: 20px;
  padding-bottom: 40px;
  gap: 40px;
  background-image: url("../../assets/img/dc-logo-bg.png");
  background-repeat: no-repeat;
  background-position: right center;
  background-size: 50%;
}

h3 {
  color: white;
  font-size: 20px;
  margin: 18px 0 10px;
}

a {
  color: $footer-mid-link;
}

li {
  margin-bottom: 10px;
}
</style>
