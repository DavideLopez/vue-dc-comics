<template>
    <div class="card">
        <img :src="src" :alt="title">
        <h1> {{ title }} </h1>
    </div>
</template>

<script>
    export default {
        props: {
            src: String,
            title: String
        }
    }
</script>

<style lang="scss" scoped>
     img {
        aspect-ratio: 1 / 1;
        object-fit: cover;
        object-position: top;
    }
</style>