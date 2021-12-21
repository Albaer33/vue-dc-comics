<template>
    <section>
        <img :src="imageObject.imageSource" :alt="imageObject.imageAlt">
    </section>
</template>

<script>
export default {
    name: 'Banner',
    props: ['imageObject']
}
</script>

<style scoped>
img {
    width: 100%;
}
</style>