<template>
  <footer class="top">
      <div class="container">
        <div class="f__nav">
          <ul>
            <li>
              <a href="#"><img src="../../assets/img/buy-comics-digital-comics.png" alt="">digital comics</a>
            </li>
            <li>
              <a href="#"><img src="../../assets/img/buy-comics-merchandise.png" alt="">dc merchandise</a>
            </li>
              <li>
                <a href="#"><img src="../../assets/img/buy-comics-subscriptions.png" alt="">subscription</a>
              </li>
            <li>
              <a href="#"><img src="../../assets/img/buy-comics-shop-locator.png" alt="">comic shop locator</a>
            </li>
            <li>
              <a href="#"><img src="../../assets/img/buy-dc-power-visa.svg" alt="">dc power visa</a>
            </li>
          </ul>
        </div>    
      </div>
  </footer>
</template>

<script>
export default {
  name: "BaseFooterTop",
  // data() {
  //   return {
  //     links: [
  //       {
  //         text: "digital comics",
  //         url: "#",
  //       },
  //       {
  //         text: "digital comics",
  //         url: "#",
  //       },
  //       {
  //         text: "digital comics",
  //         url: "#",
  //       },
  //       {
  //         text: "digital comics",
  //         url: "#",
  //       },
  //       {
  //         text: "digital comics",
  //         url: "#",
  //       },

  //     ]
  //   }
  // }
}
</script>

<style lang="scss" scoped>
    .top {
      background-color: var(--primary_color);
      color: var(--secondary_color);
        .container {
          justify-content: center;
          padding: var(--md);
            ul {
              display: flex;
              align-items: center;
              li {
                list-style: none;
                padding: var(--s);
                a {
                  text-transform: uppercase;
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