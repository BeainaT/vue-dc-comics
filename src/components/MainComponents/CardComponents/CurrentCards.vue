<template>
    <div class="card_box">
        <img :src="img" :alt="title">
        <h6>{{title}}</h6>
    </div>
</template>

<script>
export default {
    name: "CurrentCards",
    props: {
        img: String,
        title: String,
    },
}
</script>

<style lang="scss" scoped>

    img {
        width: 100%;
    }
    h6 {
        text-transform: uppercase;
        color: var(--secondary_color);
        margin: var(--s) 0;
    }

</style>