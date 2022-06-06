<template>
  <main>
    <MainHero />
    <MainCards />
  </main>
</template>

<script>
import MainHero from "./MainComponents/MainHero.vue";
import MainCards from "./MainComponents/MainCards.vue";
export default {
  name: "BaseMain",
  components: {
    MainHero,
    MainCards,
},
};
</script>

<style lang="scss" scoped>
  main {
    width: 100%;
  }
</style>