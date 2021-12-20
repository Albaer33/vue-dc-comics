<template>
    <section class="bg-footer">
        <div class="container menu">
            <div class="single-menu" v-for="(menu,index) in footerMenus" :key="index">
                <span class="title">{{menu.title}}</span>
                <ul>
                    <li v-for="(item, j) in menu.items" :key="j">
                        <a class="link" href="#">{{item}}</a>
                    </li>
                </ul>
            </div>
            <img class="bg-dc-logo" src="../assets/img/dc-logo-bg.png" alt="">
        </div>
    </section>
</template>

<script>
export default {
    name: "FooterMenu",
    data: function() {
        return {
            footerMenus: [
                {
                    title: 'DC COMICS',
                    items: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News'
                    ]
                },
                                {
                    title: 'SHOP',
                    items: [
                        'Shop DC',
                        'Shop DC Collectibles'
                    ]
                },
                                {
                    title: 'DC',
                    items: [
                        'Terms Of Use',
                        'Privacy Policy(new)',
                        'AD choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshop',
                        'CPSC certification',
                        'Ratings',
                        'Shop help',
                        'Contact Us',
                    ]
                },
                                {
                    title: 'SITES',
                    items: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Visa',
                    ]
                },
            ]
        };
    }
}
</script>

<style scoped lang="scss">
.bg-footer {
    position: relative;
    overflow: hidden;
    height: 350px;
    display: flex;
    background-image: url(../assets/img/footer-bg.jpg);
}
.menu {
    position: relative;
    padding: 30px 0;
    display: flex;
    justify-content: flex-start;
    .single-menu {
        margin-right: 30px;
    }
}
.link {
    font-size: 14px;
    text-decoration: none;
    color: grey;
}
.title {
    display: block;
    color: white;
    font-size: 20px;
    font-weight: bold;
    padding-bottom: 10px;
}
.bg-dc-logo {
    position: absolute;
    width: 400px;
    right: 50px;
    top: -50px
}
</style>