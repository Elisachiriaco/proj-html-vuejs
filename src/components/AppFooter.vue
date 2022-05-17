<template>
    <div>
        <div class="footer-up">
            <span class="subtitle">try our seasonal products</span>
            <h2>Order for pick-up or delivery to your home</h2>
            <div class="mybutton-white text-center">
            <a href="#">Shop Now</a>
          </div>
        </div>
        <div class="container footer-down" id="contact">
            <div class="row pt-4">
                <div class="col-8">
                    <img src="../assets/images/avada-bakery-logo-retina.png" alt="logo">
                </div>
                <div class="col-4">
                    <h3>Subscribe to our newsletter</h3>
                </div>
            </div>
            <div class="row">
                <div class="col-8 pt-4">
                    <ul>
                        <li v-for="(link,index) in datimyFooter" :key="index">{{link.nome}}</li>
                        <li><a href="#"><i class="fa-solid fa-cart-shopping"></i></a></li>
                    </ul>
                </div>
                <div class="col-4">
                    <div class="input-group mb-3">
                        <input type="text" class="form-control" placeholder="Enter email address*" aria-label="Enter email address" aria-describedby="basic-addon2">
                    <div class="input-group-append">
                    <span class="mybutton-violet text-center p-2">
                        <a href="#">Subscrive</a>
                    </span>
                    </div>
                    </div>
                </div>
            </div>
            <div class="row pt-4">
                <div class="col-9">
                    <ul class="copyright">
                        <li v-for="(items,index) in datiCopyright" :key="index">{{items.title}}</li>
                    </ul>
                </div>
                <div class="col-3 d-flex justify-content-end">
                    <ul>
                        <li><i class="fa-brands fa-instagram"></i></li>
                        <li><i class="fa-brands fa-twitter"></i></li>
                        <li><i class="fa-brands fa-facebook-f"></i></li>
                        <li><i class="fa-brands fa-pinterest-p"></i></li>
                    </ul>
                </div>
            </div>
            <div class="row p-3">
                <div class="col-12 d-flex justify-content-end">
                    <div class="arrow-up">
                        <a href="#home"><i class="fa-solid fa-chevron-up"></i></a>
                    </div>
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
    margin-top: 120px;
    padding: 50px 200px;
    background-image: url(../assets/images/call-to-action-bg.jpg);
    background-size: cover;
    height: 300px;
    width: 100%;
}
img{
    width: 20%;
}
li{
  list-style-type: none;
  display: inline;
  padding-right: 14px;
  color: $daisy;
  a{
    color: $daisy;
    text-decoration: none;
  }
}
.copyright{
    font-size: 8px;
    li{
        color: $grey;
        padding: 0px;
    }
}
.arrow-up{
    background-color: rgba($color: $black, $alpha: 0.4);
    width: 40px;
    height: 40px;
    text-align: center;
    line-height: 40px;
    border-radius: 50%;
    position: fixed;
    bottom: 5px;
    right: 10px;
    i{
        color: $white;
    }
}
</style>
