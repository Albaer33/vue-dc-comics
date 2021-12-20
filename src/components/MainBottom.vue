<template>
    <section>
        <div class="container">
            <ul>
                <li v-for="(service, index) in services" :key="index">
                    <img :src="service.imgSource">
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: "MainBottom",
    data: function() {
        return {
            services: [
                {
                    imgSource: '../assets/img/buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS',
                    url: '#',
                },
                {
                    imgSource: '../assets/img/buy-comics-merchandise.png',
                    text: 'DIGITAL COMICS',
                    url: '#',
                },
                {
                    imgSource: '../assets/img/buy-comics-shop-locator.png',
                    text: 'DIGITAL COMICS',
                    url: '#',
                },
                {
                    imgSource: '../assets/img/buy-comics-subscriptions.png',
                    text: 'DIGITAL COMICS',
                    url: '#',
                },
                {
                    imgSource: '../assets/img/buy-dc-power-visa.svg',
                    text: 'DIGITAL COMICS',
                    url: '#',
                },
            ],
        };
    }
}
</script>

<style scoped lang="scss">
@import '../style/variables.scss';

section {
    background-color: $brand_primary_color;
    height: 200px;
}
</style>