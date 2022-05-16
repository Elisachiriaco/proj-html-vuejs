<template>
    <div class="container">
        <section>
            <div class="row">
                <div class="col-4">
                    <span class="subtitle">Our products</span>
                    <h3>All our delectable pastries are backed fresh in our Kitchen very morning,and are made with all-natural, all organic ingredients.</h3>
                    <div class="mybutton-violet text-center">
                        <a href="#">Start Shopping</a>
                    </div>
                </div>
                <div class="col-8 d-flex flex-nowrap cookies justify-content-end">
                    <img src="../assets/images/choco-chip-cookies-400x510.jpg" alt="cookies">
                    <div class="arrow-left">
                        <i class="fa-solid fa-angle-left"></i>
                    </div>
                    <div class="arrow-right">
                        <i class="fa-solid fa-angle-right"></i>
                    </div>
                    <img src="../assets/images/strawberry-jam-cookies-400x510.jpg" alt="cookies">
                </div>
            </div>

            <div class="row pt-4">
                <div class="col-12 justify-content-center text-center">
                    <span class="subtitle">Corporate & weddings</span>
                    <h3>Baking Special Moments</h3>
                </div>
                <div class="col-6 wedding justify-content-start pt-2">
                    <img src="../assets/images/corporate-bg.jpg" alt="wedding">
                </div>
                <div class="col-6 wedding justify-content-end pt-2">
                    <img src="../assets/images/wedding-bg.jpg" alt="wedding">
                </div>
            </div>

            <div class="row shop">
                <div class="col-4 text-center justify-content-center">
                    <h3>Find a freshly baked product perfect for you </h3>
                    <p>Integer a nihb vitae ex porttitor rutrum et ut velit. Etiam ac felis at leo feugiat placerat. Sed ac nulla id orci tempor convallis sed.</p>
                    <div class="mybutton-violet text-center">
                        <a href="#">Shop All Products</a>
                    </div>
                </div>
                <div class="col-8 d-flex flex-nowrap cookies justify-content-end">
                    <div class="arrow-left">
                        <i class="fa-solid fa-angle-left"></i>
                    </div>
                    <img src="../assets/images/choco-chip-cookies-200x255.jpg" alt="cookies">
                    <img src="../assets/images/strawberry-jam-cookies-200x255.jpg" alt="cookies">
                    <img src="../assets/images/strawberry-donut-200x255.jpg" alt="donuts">
                    <img src="../assets/images/perfect-macarons-200x255.jpg" alt="macarons">
                    <div class="arrow-right">
                        <i class="fa-solid fa-angle-right"></i>
                    </div>
                </div>
            </div>

            <div class="row">
                <div class="col-3 justify-content-end">
                    <h4>Choco Chip Cookies</h4>
                    <span>$19.00 - $39.00</span>
                </div>
                <div class="col-3 justify-content-end">
                    <h4>Choco Chip Cookies</h4>
                    <span>$19.00 - $39.00</span>
                </div>
                <div class="col-3 justify-content-end">
                    <h4>Choco Chip Cookies</h4>
                    <span>$19.00 - $39.00</span>
                </div>
                <div class="col-3 justify-content-end">
                    <h4>Choco Chip Cookies</h4>
                    <span>$19.00 - $39.00</span>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    name:'AppMain'
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';
h3{
    color: $daisy;
    padding-bottom: 15px;
}
.cookies{
    position: relative;
    img{
        width: 350px;
        padding: 5px;
        margin-bottom: 20px;
    }
}
section{
    margin-top: 100px;
}

.arrow-left{
    position: absolute;
    top: 42%;
    left: 53px;
    width: 30px;
    height: 60px;
    line-height: 60px;
    background-color: rgba($color: $perfume, $alpha: 8.0);
    color: $white;
    text-align: center;
}
.arrow-right{
    position: absolute;
    top: 42%;
    right: 16px;
    width: 30px;
    height: 60px;
    line-height: 60px;
    background-color: rgba($color: $perfume, $alpha: 8.0);
    color: $white;
    text-align: center;
}

.wedding img{
    width: 100%;
    padding-left: 20px;
}

.shop{
    margin-top: 20px;
    img{
    width: 175px;
}
}
</style>