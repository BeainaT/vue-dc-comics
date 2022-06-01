<template>
  <header class="header">
      <div class="container">
        <div class="header__logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <div class="header__nav">
            <ul>
                <li v-for="(link, index) in links" :key="index"><a :href="link.url">{{link.text}}</a></li>
            </ul>
        </div>
      </div>
  </header>
</template>

<script>
export default {
    name: "baseHeader",
    data() {
        return {
            links: [
                {
                    text: "characters",
                    url: "#",
                },
                {
                    text: "comics",
                    url: "#",
                },
                {
                    text: "movies",
                    url: "#",
                },
                {
                    text: "tv",
                    url: "#",
                },
                {
                    text: "games",
                    url: "#",
                },
                {
                    text: "collectibles",
                    url: "#",
                },
                {
                    text: "videos",
                    url: "#",
                },
                {
                    text: "fans",
                    url: "#",
                },
                {
                    text: "news",
                    url: "#",
                },
                {
                    text: "shop",
                    url: "#",
                }

        ]}
    }
}
</script>

<style lang="scss" scoped>
    .container {
        justify-content: space-between;
        align-items: center;
    }
    .header {
        padding: var(--s);
        &__nav {
           ul {
               display: flex;
               list-style: none;
               li {
                   padding: var(--s);
                   a {
                       text-transform: uppercase;
                       color: var(--header_link);
                       font-weight: bold;
                   }
               }
           }
        }
    }
</style>