<template>
    <div class="card">
    <section>
        <div class="row mind p-3">
            <div class="col-12">
                <h2>Tell us what you have in mind</h2>
                <div class="number">01</div>
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
                <span>Baked to order & gift wrapped</span>
                <p>Cras consequat lectus vestibulum tortor pulvinar,quis euismod nisl varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat, finibus in velit placerat,rutrum augue.</p>
            </div>
        </div>
    </section>

    <section>
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
            <div class="col-6 newyork-subtitle">
                <h3 class="text-center">New York</h3>
                <div class="col">
                    <span class="subtitle">Call us <br> 1.800.458.556</span>
                </div>
                <div class="col">
                    <span class="subtitle">Open all week <br>9.00 am - 6.00 pm </span>
                </div>
                <div class="col">
                    <div class="mybutton-white"><a href="#"></a>View Map</div> 
                </div>
            </div>
            <div class="col-6 london-subtitle">
                <h3 class="text-center">London</h3>
                <div>

                </div>
            </div>
        </div>
    </section>

    <section>
        <div class="row">
            <div class="col-3 justify-content-start">
                <img src="../assets/images/social-1.jpg" alt="">
            </div>
            <div class="col-6 social-instagram">
                
            </div>
            <div class="col-3 justify-content-end">
                <img src="../assets/images/social-2.jpg" alt="">
            </div>
        </div>
        <div class="row">
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
    background-image: url(../assets/images/bakery-process-1.jpg);
    background-size: cover;
    height: 400px;
    position: relative;
}
.baking{
    background-image: url(../assets/images/bakery-process-2.jpg);
    background-size: cover;
    height: 400px;
    position: relative;
}
.activity{
    background-color: $pearl;
}
.delivered{
    background-image: url(../assets/images/bakery-process-3.jpg);
    background-size: cover;
    height: 400px;
    position: relative;
}
.number{
    position: absolute;
    top: 10px;
    right: 10px;
}
h2, p , .number{
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
    height: 100px;
}
.london-subtitle{
    background-color: rgba($color: $chalky, $alpha: 0.2);
    height: 100px;
}
.social-instagram{
    background-color: rgba($color: $pearl, $alpha: 0.8);
}
</style>
