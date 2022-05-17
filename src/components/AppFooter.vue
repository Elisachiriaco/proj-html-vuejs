<template>
    <div>
        <div class="footer-up">
            <span class="subtitle">try our seasonal products</span>
            <h2>Order for pick-up or delivery to your home</h2>
            <div class="mybutton-white text-center">
            <a href="#">Shop Now</a>
          </div>
        </div>
        <div class="container">
            <div class="row">
                <div class="col-8">
                    <img src="../assets/images/avada-bakery-logo-retina.png" alt="logo">
                </div>
                <div class="col-4">
                    <h3>Subscribe to our newsletter</h3>
                </div>
            </div>
            <div class="row">
                <div class="col-8">
                    <ul>
                        <li v-for="(link,index) in datimyFooter" :key="index">{{link.nome}}</li>
                        <li><a href="#"><i class="fa-solid fa-cart-shopping"></i></a></li>
                    </ul>
                </div>
                <div class="col-4">
                    <div class="input-group mb-3">
                        <input type="text" class="form-control" placeholder="Enter email address*" aria-label="Enter email address" aria-describedby="basic-addon2">
                    <div class="input-group-append">
                        <button class="btn btn-outline-secondary" type="button">Subscrive</button>
                    </div>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-8">
                    <ul class="copyright">
                        <li v-for="(items,index) in datiCopyright" :key="index">{{items.title}}</li>
                    </ul>
                </div>
                <div class="col-4">
                    <ul>
                        <li><i class="fa-brands fa-instagram"></i></li>
                        <li><i class="fa-brands fa-twitter"></i></li>
                        <li><i class="fa-brands fa-facebook-f"></i></li>
                        <li><i class="fa-brands fa-pinterest-p"></i></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'AppFooter',
    props: ["datimyFooter","datiCopyright"],
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss'; 

.footer-up{
    background-image: url(../assets/images/call-to-action-bg.jpg);
    background-size: cover;
    height: 300px;
    width: 100%;
}
img{
    width: 20%;
}
.copyright{
    font-size: 8px;
    li{
        color: $grey;
        padding: 0px;
    }
}
</style>
