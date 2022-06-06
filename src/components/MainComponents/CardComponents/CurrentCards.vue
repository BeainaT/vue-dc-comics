<template>
    <div class="card_box">
        <img :src="img" :alt="title">
        <h3>{{title}}</h3> 
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

<style>

</style>