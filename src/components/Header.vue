<template>
    <header class="container">
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="logo dc">
        </div>
        <ul>
            <li class="item" v-for="(link, index) in links" :key="index">
                <a class="menu-btn" :href="link.url">{{link.text}}</a>
            </li>
        </ul>
    </header>
</template>

<script>
    export default {
    name: "Header",
    data: function() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    current: false
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    current: false
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    current: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    current: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    current: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    current: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    current: false
                },
            ],
        };
    }
}
</script>

<style scoped lang="scss">
@import '../style/variables.scss';

header {
    display: flex;
    justify-content: space-between;
    height: 120px;
    line-height: 120px;
    ul {
        list-style-type: none;
        display: flex;
    }
}
.menu-btn {
    display: block;
    margin: 0 10px;
    color: black;
    text-decoration: none;
    &:hover {
        border-bottom: 4px solid $brand_primary_color;
    }
}
.logo {
    display: flex;
    align-items: center;
    height: 100%;
    img {
        height: 80px;
    }
}
</style>
