<template>
    <section>
        <div class="container">
            <ul>
                <li v-for="(service, index) in services" :key="index">
                    <img :src="require('../assets/img/'+service.img)">
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
                    img: 'buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS',
                },
                {
                    img: 'buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE',
                },
                {
                    img: 'buy-comics-shop-locator.png',
                    text: 'COMIC SHOP LOCATOR',
                },
                {
                    img: 'buy-comics-subscriptions.png',
                    text: 'SUBSCRIPTION',
                },
                {
                    img: 'buy-dc-power-visa.svg',
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
    ul {
        padding: 50px 0;
        display: flex;
        justify-content: space-between;
        li {
            width: calc(100% / 5);
            color: white;
            display: flex;
            align-items: center;
            width: 50px;
            span {
                padding: 0 10px;
            }
        }
    }
}
</style>