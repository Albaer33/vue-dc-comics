<template>
    <section>
        <div class="container">
            <ul>
                <li v-for="(service, index) in services" :key="index">
                    <img :src="require(service.imgSource)">
                    <span>{{service.text}}</span>
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
                },
                {
                    imgSource: '../assets/img/buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE',
                },
                {
                    imgSource: '../assets/img/buy-comics-shop-locator.png',
                    text: 'COMIC SHOP LOCATOR',
                },
                {
                    imgSource: '../assets/img/buy-comics-subscriptions.png',
                    text: 'SUBSCRIPTION',
                },
                {
                    imgSource: '../assets/img/buy-dc-power-visa.svg',
                    text: 'DC POWER VISA',
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