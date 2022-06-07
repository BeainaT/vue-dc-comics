<template>
    <div class="card_box">
        <div class="img_box">
            <img :src="img" :alt="title" />
        </div>
        <h6>{{ title }}</h6>
    </div>
</template>

<script>
export default {
  name: "CurrentCards",
  props: {
    img: String,
    title: String,
  },
};
</script>

<style lang="scss" scoped>
.card_box {
      text-align: left;
      max-width: 12.5rem;
      .img_box {
          width: 12.5rem;
          height: 12.5rem;
          overflow: hidden;
          img {
              width: 100%;
          }
      }

  h6 {
    text-transform: uppercase;
    color: var(--secondary_color);
    margin: var(--s) 0;
  }
}
</style>