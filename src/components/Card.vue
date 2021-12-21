<template>
    <div class="card">
        <img :src="cardObject.thumb" :alt="cardObject.series">
        <h3>{{cardObject.series}}</h3>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: ['cardObject']
}
</script>

<style scoped lang="scss">
.card {
    width: calc((100% / 6) - 20px);
    margin: 10px;
    h3 {
        padding: 10px 0;
    }
}
</style>