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
                    <span class="mybutton-violet text-center px-4 py-2">
                        <a href="#">Shop All Products</a>
                    </span>
                </div>
                <div class="col-8 d-flex flex-nowrap cookies justify-content-end">
                    <div class="smarrow-left">
                        <i class="fa-solid fa-angle-left"></i>
                    </div>
                <div>
                    <img src="../assets/images/choco-chip-cookies-200x255.jpg" alt="cookies">
                    <h4>Choco Chip Cookies</h4>
                    <p class="price">$19.00 - $39.00</p>
                </div>
                <div>
                    <img src="../assets/images/strawberry-jam-cookies-200x255.jpg" alt="cookies">
                    <h4>Strawberry Jam Cookies</h4>
                    <p class="price">$24.00 - $62.00</p>
                </div>
                <div>
                    <img src="../assets/images/strawberry-donut-200x255.jpg" alt="donuts">
                    <h4>Strawberry Donut</h4>
                    <p class="price">$24.00 - $42.00</p>
                </div>
                <div>
                    <img src="../assets/images/perfect-macarons-200x255.jpg" alt="macarons">
                    <h4>Perfect Macarons</h4>
                    <p class="price">$18.00 - $52.00</p>
                    <div class="smarrow-right">
                        <i class="fa-solid fa-angle-right"></i>
                    </div>
                </div>
                </div>
            </div>
        </section>
        <app-card />
    </div>
</template>

<script>
import AppCard from './AppCard.vue'
export default {
    name:'AppMain',
    components: {
        AppCard
    }
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
    background-color: rgba($color: $perfume, $alpha: 0.7);
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
    background-color: rgba($color: $perfume, $alpha: 0.7);
    color: $white;
    text-align: center;
}

.smarrow-left{
    position: absolute;
    top: 30%;
    left: 53px;
    width: 20px;
    height: 50px;
    line-height: 50px;
    background-color: rgba($color: $perfume, $alpha: 0.7);
    color: $white;
    text-align: center;
    i{
        font-size: 8px;
    }
}

.smarrow-right{
    position: absolute;
    top: 30%;
    right: 16px;
    width: 20px;
    height: 50px;
    line-height: 50px;
    background-color: rgba($color: $perfume, $alpha: 0.7);
    color: $white;
    text-align: center;
    i{
        font-size: 8px;
    }
}


.wedding img{
    width: 100%;
    padding-left: 20px;
}

.shop{
    margin-top: 120px;
    margin-bottom: 80px;
    img{
    width: 175px;
    }
}
h4{
    font-size: 12px;
    color: $daisy;
    text-align: center;
    font-weight: 700;
}
.price{
    text-align: center;
    font-size: 10px;
    color: $daisy;
}

</style> 