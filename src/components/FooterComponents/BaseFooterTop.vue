<template>
  <div class="top">
    <div class="container py-4">
      <ul class="p-0 m-0">
        <li v-for="(link, index) in links" :key="index">
          <a :href="link.url"
            ><img :src="link.img" :alt="link.title" />{{link.text}}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "BaseFooterTop",
  data() {
    return {
      links: [
        {
          img: require("../../assets/img/buy-comics-digital-comics.png"),
          text: "digital comics",
          title: "screen with logo",
        },
        {
          img: require("../../assets/img/buy-comics-merchandise.png"),
          text: "dc merchandise",
          title: "t-shirt",
        },
        {
          img: require("../../assets/img/buy-comics-subscriptions.png"),
          text: "subscription",
          title: "cards",
        },
        {
          img: require("../../assets/img/buy-comics-shop-locator.png"),
          text: "comic shop locator",
          title: "locator icon",
        },
        {
          img: require("../../assets/img/buy-dc-power-visa.svg"),
          text: "dc power visa",
          title: "shop card",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/mixins.scss";

.top {
  background-color: var(--primary_color);
  color: var(--secondary_color);

  ul {
    @include flex("around");

    li {
      padding: var(--s);

      a {
        @include flex;
        gap: var(--s);
        color: var(--secondary_color);

        img {
          max-width: var(--lg);
          height: var(--lg);
        }
      }
    }
  }
}
</style>