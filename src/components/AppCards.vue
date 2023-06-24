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
        <div id="title">
            {{ title }}
        </div>
    </div>
</template>

<style lang="scss" scoped>
img{
    aspect-ratio: 3/4;
    object-fit: cover;
    max-width: 100%;
}
#title{
    color: white;
    text-transform: uppercase;
    font-size: 12px;
    margin-top: 1em;
}
</style>