<template>
  <div class="footer__bottom py-4">
    <div class="container">
      <button class="btn btn_custom">sign-up now!</button>
      <div class="social">
        <span>follow us</span>
        <ul class="p-0 m-0">
          <li v-for="(social, index) in socialMedia" :key="index">
            <a :href="social.url"
              ><img :src="social.img" :alt="social.title" /></a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BaseFooterBottom",
  data() {
    return {
      socialMedia: [
        {
          img: require("../../assets/img/footer-facebook.png"),
          url: "#",
          title: "facebook",
        },
        {
          img: require("../../assets/img/footer-twitter.png"),
          url: "#",
          title: "twitter",
        },
        {
          img: require("../../assets/img/footer-youtube.png"),
          url: "#",
          title: "youtube",
        },
        {
          img: require("../../assets/img/footer-pinterest.png"),
          url: "#",
          title: "pinterest",
        },
        {
          img: require("../../assets/img/footer-periscope.png"),
          url: "#",
          title: "periscope",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/mixins.scss";
.footer__bottom {
  background-color: var(--footer_bg_color);
  color: var(--primary_color);
  text-transform: uppercase;
  .container {
    @include flex("between");
    .btn_custom {
      border: 0.125rem solid var(--primary_color);
      background-color: inherit;
      &:hover {
        background-color: var(--primary_color);
        transition: 0.3s linear;
      }
    }
    .social {
      @include flex;
      gap: var(--s-m);
      font-size: var(--s-m);
      font-weight: bold;
      ul {
        @include flex;
        gap: var(--s);
        a:hover {
          opacity: 0.8;
        }
      }
    }
  }
}
</style>