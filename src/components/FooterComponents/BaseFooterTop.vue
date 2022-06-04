<template>
  <div class="top">
    <div class="container py-4">
      <div class="f__nav">
        <ul class="p-0 m-0">
          <li>
            <a href="#"><img src="../../assets/img/buy-comics-digital-comics.png" alt="" />digital comics</a>
          </li>
          <li>
            <a href="#"><img src="../../assets/img/buy-comics-merchandise.png" alt="" />dc merchandise</a>
          </li>
          <li>
            <a href="#"><img src="../../assets/img/buy-comics-subscriptions.png" alt="" />subscription</a>
          </li>
          <li>
            <a href="#"><img class="locator" src="../../assets/img/buy-comics-shop-locator.png" alt="" />comic shop locator</a>
          </li>
          <li>
            <a href="#"><img src="../../assets/img/buy-dc-power-visa.svg" alt="" />dc power visa</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BaseFooterTop",
};
</script>

<style lang="scss" scoped>
.top {
  background-color: var(--primary_color);
  color: var(--secondary_color);

  .container {
    justify-content: center;

    ul {
      display: flex;
      align-items: center;
      flex-wrap: wrap;
      justify-content: space-around;

      li {
        padding: var(--s);

        a {
          display: flex;
          align-items: center;
          gap: var(--s);
          color: var(--secondary_color);

          img {
            width: var(--lg);
          }
        }
      }
    }
  }
}
</style>