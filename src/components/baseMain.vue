<template>
  <main>
    <MainHero />
  </main>
</template>

<script>
import MainHero from "./MainComponents/MainHero.vue";
export default {
  name: "BaseMain",
  components: {
    MainHero,
  },
};
</script>

<style lang="scss" scoped>
  main {
    width: 100%;
  }
</style>