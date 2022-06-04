<template>
  <div class="footer__bottom py-4">
      <div class="container">
          <button class="btn btn_custom">sign-up now!</button>
          <div class="social">
              <span>follow us</span>
              <a href=""><img src="../../assets/img/footer-facebook.png" alt=""></a>
              <a href=""><img src="../../assets/img/footer-twitter.png" alt=""></a>
              <a href=""><img src="../../assets/img/footer-youtube.png" alt=""></a>
              <a href=""><img src="../../assets/img/footer-pinterest.png" alt=""></a>
              <a href=""><img src="../../assets/img/footer-periscope.png" alt=""></a>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "BaseFooterBottom"
}
</script>

<style lang="scss" scoped>
    .footer__bottom {
        background-color: var(--footer_bg_color);
        color: var(--primary_color);
        text-transform: uppercase;
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            .btn_custom {
                border: 0.125rem solid var(--primary_color);
                border-radius: 0;
                color: var(--secondary_color);
            }
            .social {
                display: flex;
                flex-wrap: wrap;
                align-items: center;
                gap: var(--s-m);
                font-size: var(--s-m);
                font-weight: bold;
            }
        }
    }
</style>