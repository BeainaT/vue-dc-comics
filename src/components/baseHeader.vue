<template>
  <header class="header">
    <div class="container">
      <div class="header__logo">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>
      <div class="header__nav">
        <ul class="p-0 m-0">
          <li v-for="(link, index) in links" :key="index">
            <a :class="{active : link.isActive}" :href="link.url" @mouseover="activeLink(link)" @mouseleave="activeLink(link)">{{ link.text }}</a>
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
          isActive: false,
        },
        {
          text: "comics",
          url: "#",
          isActive: false,
        },
        {
          text: "movies",
          url: "#",
          isActive: false,
        },
        {
          text: "tv",
          url: "#",
          isActive: false,
        },
        {
          text: "games",
          url: "#",
          isActive: false,
        },
        {
          text: "collectibles",
          url: "#",
          isActive: false,
        },
        {
          text: "videos",
          url: "#",
          isActive: false,
        },
        {
          text: "fans",
          url: "#",
          isActive: false,
        },
        {
          text: "news",
          url: "#",
          isActive: false,
        },
        {
          text: "shop",
          url: "#",
          isActive: false,
        },
      ],
      
    }
  },
  methods: {
    activeLink(obj) {
      obj.isActive = !obj.isActive;
    }
  }
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

        &.active {
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