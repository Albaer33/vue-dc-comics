<template>
    <div class="img-container">
        <img :src="imageObject.imageSource" :alt="imageObject.imageAlt">
    </div>
</template>

<script>
export default {
    name: 'Banner',
    props: ['imageObject']
}
</script>

<style scoped>
.img-container {
    width: 100%;
    height: 500px;
}
img {
    width: 100%;
    height: 200px;
}
</style>