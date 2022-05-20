<template>
    <div class="container">
        <section id="shop">
            <div class="row">
                <div class="col-4"         
                data-aos="zoom-in-left"
                data-aos-duration="1000"
                data-aos-offset="0"
                data-aos-delay="500"
                data-aos-id="super-duper">
                    <span class="subtitle">Our products</span>
                    <h3>All our delectable pastries are backed fresh in our Kitchen very morning,and are made with all-natural, all organic ingredients.</h3>
                    <div class="mybutton-violet text-center">
                        <a href="#">Start Shopping</a>
                    </div>
                </div>
                <div class="col-8 d-flex flex-nowrap cookies justify-content-end"
                data-aos="zoom-in-left"
                data-aos-duration="1000"
                data-aos-offset="0"
                data-aos-delay="500"
                data-aos-id="super-duper">
                    <div 
                    tabindex="0" @muoseleave="autoScroll" @mouseover="stopAutoScroll">
                    <img :src="datimySlider[activeIndex].image" alt="cookies">
                    <img :src="datimySlider[activeIndex].secondImage" alt="cookies">
                    </div>
                    <div class="hover-cookies justify-content-center text-center align-items-center">
                        <div class="text-cookies">
                        <h5>Choco Chip Cookies</h5>
                        <span>Cookies Pastries</span>
                        <p>$19.00 - 39.00</p>
                        </div>
                    </div> 
                    <div class="hover-cookiesrg justify-content-center text-center align-items-center">
                        <div class="text-cookies">
                        <h5>Strawberry Jam Cookies</h5>
                        <span>Cookies Pastries</span>
                        <p>$24.00 - $62.00</p>
                        </div>
                    </div>
                    <div class="col">
                    <div class="arrow-left" @click="prevSlide(activeIndex)">
                        <i class="fa-solid fa-angle-left"></i>
                    </div>
                    <div class="arrow-right" @click="nextSlide(activeIndex)">
                        <i class="fa-solid fa-angle-right"></i>
                    </div>
                </div>
                </div>
            </div>
        </section>
        <section id="about">
            <div class="row pt-4">
                <div class="col-12 justify-content-center text-center">
                    <span class="subtitle">Corporate & weddings</span>
                    <h3>Baking Special Moments</h3>
                </div>
            </div>
            <div class="row">
                <div class="col-6 event pt-2 justify-content-center" 
                data-aos="fade-up"
                data-aos-duration="2000"
                data-aos-offset="0"
                data-aos-delay="1000"
                data-aos-id="super-duper">
                    <img class="img-hover" src="../assets/images/corporate-hover-bg.jpg" alt="">
                    <div class="text-hover text-center">
                    <span>International Bakery</span>
                    <h5>Corporate Events</h5>
                    <div class="mybutton-violet text-center">
                        <a href="#">Explore more</a>
                    </div>
                    </div>
                </div>
                <div class="col-6 wedding pt-2 justify-content-center"
                data-aos="fade-up"
                data-aos-duration="1000"
                data-aos-offset="0"
                data-aos-delay="500"
                data-aos-id="super-duper">
                    <img class="img-hover" src="../assets/images/wedding-hover-bg.jpg" alt="">
                    <div class="text-hover text-center">
                    <span>Private dining hall</span>
                    <h5>Wedding & Parties</h5>
                    <div class="mybutton-violet text-center">
                        <a href="#">Explore more</a>
                    </div>
                    </div>
                </div>
            </div>

            <div class="row shop"
                data-aos="zoom-in-right"
                data-aos-duration="2000"
                data-aos-offset="0"
                data-aos-delay="1000"
                data-aos-id="super-duper"
                tabindex="0" @muoseleave="autoScroll" @mouseover="stopAutoScroll">
                <div class="col-4 text-center justify-content-center">
                    <h3>Find a freshly baked product perfect for you </h3>
                    <p>Integer a nihb vitae ex porttitor rutrum et ut velit. Etiam ac felis at leo feugiat placerat. Sed ac nulla id orci tempor convallis sed.</p>
                    <span class="mybutton-violet text-center px-4 py-2">
                        <a href="#">Shop All Products</a>
                    </span>
                </div>
                <div class="col-8 d-flex flex-nowrap cookies justify-content-end">
                    <div class="smarrow-left" @click="prevSlide(activeIndex)">
                        <i class="fa-solid fa-angle-left"></i>
                    </div>
                <div>
                    <img :src="datiSecondSlider[activeIndex].img" alt="cookies">
                    <h4>{{datiSecondSlider[activeIndex].title}}</h4>
                    <p class="price">{{datiSecondSlider[activeIndex].price}}</p>
                </div>
                <div>
                    <img :src="datiSecondSlider[activeIndex].secondImg" alt="cookies">
                    <h4>{{datiSecondSlider[activeIndex].secondTitle}}</h4>
                    <p class="price">{{datiSecondSlider[activeIndex].secondPrice}}</p>
                </div>
                <div>
                    <img :src="datiSecondSlider[activeIndex].thirdImg" alt="donuts">
                    <h4>{{datiSecondSlider[activeIndex].thirdTitle}}</h4>
                    <p class="price">{{datiSecondSlider[activeIndex].thirdPrice}}</p>
                </div>
                <div>
                    <img :src="datiSecondSlider[activeIndex].fourthImg" alt="macarons">
                    <h4>{{datiSecondSlider[activeIndex].fourthTitle}}</h4>
                    <p class="price">{{datiSecondSlider[activeIndex].fourthPrice}}</p>
                    <div class="smarrow-right" @click="nextSlide(activeIndex)">
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
    },
    props : ["datimySlider", "datiSecondSlider"],
    data(){
        return{
            activeIndex : 0,
            intervalId : null 
        }
    },
      methods: {
        nextSlide(){
            this.activeIndex = (this.activeIndex === 1) ? 0 : this.activeIndex +=1;
        },
        prevSlide(){
            this.activeIndex = (this.activeIndex === 0) ? 1 : this.activeIndex -=1;
        },
        autoScroll(){
            this.intervalId = setInterval(()=>{
            this.nextSlide();
            },2000)
        },
        stopAutoScroll(){
            clearInterval(this.intervalId);
            this.intervalId = null;
        },
    },
    mounted(){
      this.autoScroll()
    }
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';
.cookies{
    position: relative;
    transition-duration: 2s;
    img{
        width: 350px;
        padding: 5px;
        margin-bottom: 20px;
    }
}
// .cookies:hover .hover-cookies{
//     display: inline-block;
//     transition: all 2s;
// }
// .cookies:hover .hover-cookiesrg{
//     display: inline-block;
// }
.text-cookies{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
}
.hover-cookies{
    position: absolute;
    top: 5px;
    left: 15px;
    z-index: 30;
    color: $white;
    display: none;
    background: linear-gradient(90deg, rgba(0,0,0,0.2) 0%, rgba(0,0,0,0.4) 35%, rgba(0,0,0,0.6) 100%);
    width: 340px;
    height: 94%;
}
.hover-cookiesrg{
    position: absolute;
    top: 5px;
    right: 50px;
    width: 340px;
    height: 94%;
    display: none;
    background: linear-gradient(90deg, rgba(0,0,0,0.6) 0%, rgba(0,0,0,0.4) 35%, rgba(0,0,0,0.2) 100%);
    color: $white;
    z-index: 30;
}
section{
    margin-top: 100px;
}

.arrow-left{
    position: absolute;
    top: 42%;
    left: 15px;
    width: 30px;
    height: 60px;
    line-height: 60px;
    background-color: rgba($color: $perfume, $alpha: 0.7);
    color: $white;
    text-align: center;
    cursor: pointer;
    &:hover{
        background-color: $perfume;
    }
}
.arrow-right{
    position: absolute;
    top: 42%;
    right: 50px;
    width: 30px;
    height: 60px;
    line-height: 60px;
    background-color: rgba($color: $perfume, $alpha: 0.7);
    color: $white;
    text-align: center;
    cursor: pointer;
    &:hover{
        background-color: $perfume;
    }
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
    cursor: pointer;
    i{
        font-size: 8px;
    }
    &:hover{
        background-color: $perfume;
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
    cursor: pointer;
    i{
        font-size: 8px;
    }
    &:hover{
        background-color: $perfume;
    }
}


.event{
    background-image: url(../assets/images/corporate-bg.jpg);
    background-size:contain;
    background-repeat: no-repeat;
    position: relative;
    height: 500px;
    transition: 1s ease-in-out;
}
.event:hover .img-hover{
    display: inline-block;
}
.wedding:hover .img-hover{
    display: inline-block;
}
.wedding:hover .text-hover{
    display: inline-block;
}
.event:hover .text-hover{
    display: inline-block;
}
.wedding{
    background-image: url(../assets/images/wedding-bg.jpg);
    background-size: contain;
    background-repeat: no-repeat;
    position: relative;
    height:500px;
    transition: 1s ease-in-out;
}
.img-hover{
    display: none;
    position: absolute;
    top: 0;
    left: 0;
    height: 500px;
    z-index: 20;
}
.text-hover{
    display: none;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 1000;
    color: $white;
    span{
        text-transform: uppercase;
        font-size: 8px;
    }
    h5{
        font-size: 22px;
    }
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