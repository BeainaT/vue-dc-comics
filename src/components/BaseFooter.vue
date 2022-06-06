<template>
  <footer>
    <BaseFooterTop />
    <BaseFooterNav />
    <BaseFooterBottom />
  </footer>
</template>

<script>
import BaseFooterNav from "./FooterComponents/BaseFooterNav.vue";
import BaseFooterTop from "./FooterComponents/BaseFooterTop.vue";
import BaseFooterBottom from "./FooterComponents/BaseFooterBottom.vue";
export default {
  name: "BaseFooter",
  components: {
    BaseFooterNav,
    BaseFooterTop,
    BaseFooterBottom,
  },
};
</script>

<style lang="scss" scoped>
</style>