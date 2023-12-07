<script>
export default {
  data() {
    return {
      buys: [
        {
          img: "/img/buy-comics-digital-comics.png",
          text: "digital comics",
          href: "#",
          target: "_self",
        },
        {
          img: "/img/buy-comics-merchandise.png",
          text: "dc merchandise",
          href: "#",
          target: "_self",
        },
        {
          img: "/img/buy-comics-subscriptions.png",
          text: "subscription",
          href: "#",
          target: "_self",
        },
        {
          img: "/img/buy-comics-shop-locator.png",
          text: "comic shop locator",
          href: "#",
          target: "_self",
        },
        {
          img: "/img/buy-dc-power-visa.svg",
          text: "dc power visa",
          href: "#",
          target: "_self",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="footer-top">
    <div class="container">
      <ul class="flex">
        <li v-for="merch in buys" class="flex">
          <div class="img-box">
            <img :src="merch.img" alt="merch.text" />
          </div>
          <a :href="merch.href" :target="merch.target" class="upper">{{
            merch.text
          }}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped lang="scss">
@use "../../styles/_partials/utilities.scss";
@use "../../styles/_partials/container.scss";
@use "../../styles/_partials/variables.scss" as *;

.footer-top {
  background-color: $primary-color;
  ul {
    padding: 50px 40px;
    gap: 30px;
    align-items: center;
    justify-content: space-between;
    li:first-child {
      .img-box {
        width: 50px;
      }
    }
    li:nth-child(2) {
      .img-box {
        width: 55px;
      }
    }
    li:nth-child(3) {
      .img-box {
        width: 55px;
      }
    }
    li:nth-child(4) {
      .img-box {
        width: 40px;
      }
    }
    li:last-child {
      .img-box {
        width: 55px;
      }
    }
  }
}

a {
  color: white;
  font-size: 12px;
  display: block;
}

.img-box {
  margin-right: 10px;
}

li {
  align-items: center;
}
</style>
