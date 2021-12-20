<template>
    <footer class="bg-grey">
        <div class="footer-container container">
            <div class="btn">
                <a href="#">SIGN-UP NOW!</a>
                
            </div>
            <div class="social">
                <div class="text">FOLLOW US</div>
                <i class="fab fa-facebook-square icon"></i>
                <i class="fab fa-twitter icon"></i>
                <i class="fab fa-youtube icon"></i>
                <i class="fab fa-pinterest icon"></i>
                <i class="fa fa-map-marker icon" aria-hidden="true"></i>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "FooterContact"
}
</script>

<style scoped lang="scss">
@import '../style/variables.scss';

.bg-grey {
    background-color: #303030;
}
.footer-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 150px;
}
.btn {
    a {
        color: white;
        text-decoration: none;
        border: 3px solid $brand_primary_color;
        padding: 20px;
    }
}
.social {
    display: flex;
    align-items: center;
    font-size: 28px;
    .icon {
        color: #303030;
        padding: 15px;
        margin: 0 10px;
        background-color: #797979;
        border-radius: 50%;
    }
    .text {
        color: $brand_primary_color;
        margin-right: 30px;
    }
}
</style>