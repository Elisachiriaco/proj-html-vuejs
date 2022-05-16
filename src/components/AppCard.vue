<template>
    <section>
        <div class="row mind p-3">
            <div class="col-12">
                <h2>Tell us what you have in mind</h2>
                <span class="subtitle">Manual ingredients selection</span>
                <p>Cras consequat lectus vestibulum tortor pulvinar,quis euismod nisl varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat, finibus in velit placerat,rutrum augue.</p>
            </div>
        </div>
        <div class="row py-3">
            <div class="col-6 baking">
                <h2>We start baking</h2>
                <span class="subtitle">Sweet & delicious</span>
                <p>Cras consequat lectus vestibulum tortor pulvinar,quis euismod nisl varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat, finibus in velit placerat.</p>
            </div>
            <div class="col-6 activity">
                <span class="subtitle"></span>
                <h3>"Finally found an alternative to the mass produced products. Something that incorporates real organic ingredients, nutrient dense wellness while promoting sustainability and activity.</h3>
                <p>Rachel Cooper, Founder</p>
            </div>
        </div>
        <div class="row delivered p-3">
            <div class="col-12">
                <h2>Delivered to your home</h2>
                <span>Baked to order & gift wrapped</span>
                <p>Cras consequat lectus vestibulum tortor pulvinar,quis euismod nisl varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat, finibus in velit placerat,rutrum augue.</p>
            </div>
        </div>
    </section>
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
}
.baking{
    background-image: url(../assets/images/bakery-process-2.jpg);
    background-size: cover;
    height: 400px;
}
.activity{
    background-color: $pearl;
}
.delivered{
    background-image: url(../assets/images/bakery-process-3.jpg);
    background-size: cover;
    height: 400px;
}
</style>
