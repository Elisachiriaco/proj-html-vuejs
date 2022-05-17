<template>
    <div class="container">
    <section id="gallery">
        <div class="row mind p-3">
            <div class="col-12">
                <h2>Tell us what you have in mind</h2>
                <div class="number">01</div>
            </div>
            <div class="col-4">
                <span class="subtitle">Manual ingredients selection</span>
                <p>Cras consequat lectus vestibulum tortor pulvinar,quis euismod nisl varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat, finibus in velit placerat,rutrum augue.</p>
            </div>
        </div>
        <div class="row py-3">
            <div class="col-6 baking">
                <h2>We start baking</h2>
                <div class="number">02</div>
                <span class="subtitle">Sweet & delicious</span>
                <p>Cras consequat lectus vestibulum tortor pulvinar,quis euismod nisl varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat, finibus in velit placerat.</p>
            </div>
            <div class="col-6 activity">
                <span class="subtitle">Dont just take our word for it</span>
                <h3>"Finally found an alternative to the mass produced products. Something that incorporates real organic ingredients, nutrient dense wellness while promoting sustainability and activity."</h3>
                <p>Rachel Cooper, Founder</p>
            </div>
        </div>
        <div class="row delivered p-3">
            <div class="col-12">
                <h2>Delivered to your home</h2>
                <div class="number">03</div>
            </div>
            <div class="col-4">
                <span>Baked to order & gift wrapped</span>
                <p>Cras consequat lectus vestibulum tortor pulvinar,quis euismod nisl varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat, finibus in velit placerat,rutrum augue.</p>
            </div>
        </div>
    </section>

    <section id="locations">
        <div class="row">
            <div class="col-12 justify-content-center text-center">
                <span class="subtitle">Locations</span>
                <h3>Visit our Bakeries</h3>
            </div>
        </div>
        <div class="row">
            <div class="col-6 newyork"></div>
            <div class="col-6 london"></div>
        </div>
        <div class="row">
            <div class="col-6 newyork-subtitle justify-content-center">
                <h3 class="text-center pt-3">New York</h3>
                <div class="information text-center">Call us <br> 1.800.458.556 </div>
                <div class="information text-center">Open all week <br> 9.00 am - 6.00 pm</div>
                <div class="mybutton-white text-center d-inline-block">
                    <a href="#">View Map</a>
                </div>
            </div>
            <div class="col-6 london-subtitle">
                <h3 class="text-center pt-3">London</h3>
                <div class="information text-center">Call us <br> 1.800.458.556 </div>
                <div class="information text-center">Open all week <br> 9.00 am - 6.00 pm</div>
                <div class="mybutton-white text-center d-inline-block">
                    <a href="#">View Map</a>
                </div>
            </div>
        </div>
    </section>

    <section id="journal">
        <div class="row">
            <div class="col-3 justify-content-start">
                <img src="../assets/images/social-1.jpg" alt="">
            </div>
            <div class="col-6 social-instagram d-flex align-items-center">
            <div class="col-12 justify-content-center text-center">
                <span class="subtitle">Made for sharing</span>
                <h3>Let's stay in touch</h3>
                <span class="mybutton-violet px-4 py-2"><a href="#"><i class="fa-brands fa-instagram"></i>Follow us</a></span>
            </div>
            </div>
            <div class="col-3 justify-content-end">
                <img src="../assets/images/social-2.jpg" alt="">
            </div>
        </div>
        <div class="row pt-4">
            <div class="col-3">
                <img src="../assets/images/social-3.jpg" alt="">
            </div>
            <div class="col-3">
                <img src="../assets/images/social-4.jpg" alt="">
            </div>
            <div class="col-3">
                <img src="../assets/images/social-5.jpg" alt="">
            </div>
            <div class="col-3">
                <img src="../assets/images/social-6.jpg" alt="">
            </div>
        </div>
    </section>


    </div>
</template>

<script>
export default{
    name: 'AppCard',
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';
.mind{
    background-image:  linear-gradient(to bottom, rgba(0,0,0,0.5), rgba(0,0,0,0.2)),
    url(../assets/images/bakery-process-1.jpg);
    background-size: cover;
    height: 400px;
    position: relative;
}
.baking{
    background-image: linear-gradient(to bottom, rgba(0,0,0,0.5), rgba(0,0,0,0.2)),
    url(../assets/images/bakery-process-2.jpg);
    background-size: cover;
    height: 400px;
    position: relative;
}
.activity{
    background-color: $pearl;
}
.delivered{
    background-image:linear-gradient(to bottom, rgba(0,0,0,0.5), rgba(0,0,0,0.2)),
    url(../assets/images/bakery-process-3.jpg);
    background-size: cover;
    height: 400px;
    position: relative;
}
.number{
    position: absolute;
    top: 10px;
    right: 10px;
    font-size: 60px;
}
p , .number{
    color: $white;
}
img{
    width: 100%;
}

.newyork{
    background-image: url(../assets/images/new-york-bk.jpg);
    background-size: cover;
    height: 400px;
}
.london{
    background-image: url(../assets/images/london-bk.jpg);
    background-size: cover;
    height: 400px;
}
.newyork-subtitle{
    background-color: rgba($color: $atoll, $alpha: 0.1);
    height: 120px;
}
.london-subtitle{
    background-color: rgba($color: $chalky, $alpha: 0.2);
    height: 120px;
}
.social-instagram{
    background-color: rgba($color: $pearl, $alpha: 0.8);
}
#location, #social{
    margin-top: 120px;
}
.information{
    display: inline-block;
    padding: 0px 50px;
    text-transform: uppercase;
    color: $grey;
    font-size: 10px;
}
</style>
