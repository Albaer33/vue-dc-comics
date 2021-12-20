<template>
    <section class="bg-footer">
        <div class="container">
            <div v-for="(menu,index) in footerMenus" :key="index">
                {{menu.title}}
                <ul>
                    <li v-for="(item, j) in menu.items" :key="j">
                        <a href="#">{{item}}</a>
                    </li>
                </ul>
            </div>
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
</style>