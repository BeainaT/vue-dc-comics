<template>
  <button class="btn btn_custom mb-3">load more</button>
</template>

<script>
export default {
    name: "MainButton"
}
</script>

<style lang="scss" scoped>
.btn_custom {
    background-color: var(--primary_color);
    border-radius: 0;
    color: var(--secondary_color);
    padding: var(--xs) var(--lg);
    font-weight: bold;
}
</style>