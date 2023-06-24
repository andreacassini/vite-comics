<script>
export default {
    props:{
        image: String,
        title: String
    }
}
</script>

<template>
    <div>
        <img :src="image" alt="card">
        <h1>{{ title }}</h1>
    </div>
</template>

<style lang="scss">
img{
    aspect-ratio: 3/4;
    object-fit: cover;
    max-width: 100%;
}
</style>