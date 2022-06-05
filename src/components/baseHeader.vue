<template>
  <header class="header">
    <div class="container">
      <div class="header__logo">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>
      <div class="header__nav">
        <ul class="p-0 m-0">
          <li v-for="(link, index) in links" :key="index">
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "BaseHeader",
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
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/mixins.scss";

.container {
  @include flex("between");

  ul {
    @include flex;

    li {
      padding: var(--lg) 0;
      margin: 0 var(--s);
      position: relative;

      a {
        color: var(--header_link);
        font-weight: bold;

        &:hover {
          color: var(--primary_color);

          &::after {
            content: "";
            display: block;
            height: var(--xs);
            width: 100%;
            position: absolute;
            bottom: 0;
            background-color: var(--primary_color);
            text-align: center;
          }
        }
      }
    }
  }
}
</style>