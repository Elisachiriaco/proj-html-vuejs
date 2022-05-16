<template>
    <div class="container">
      <div class="row align-items-center">
        <div class="col-4 justify-content-start">
          <img src="../assets/images/avada-bakery-logo-retina.png" alt="logo">
        </div>
        <div class="col-8 justify-content-end">
        <ul>
          <li v-for="(item, index) in datimyNav" :key="index">{{item.nome}}</li>
          <li><a href="#"><i class="fa-solid fa-cart-shopping"></i></a></li>
        </ul>
      </div>
      <div class="row header-bg">
        <div class="col-4">
          <span class="subtitle">Fresh & tasty bakery every day</span>
          <h1>The Perfect Fresh Bread</h1>
          <p>Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius. Aliquam erat volutpat. Nullam quis sagittis nibh ac nulla id orci tempor.</p>
          <div class="mybutton-white text-center">
            <a href="#">Explore our products</a>
          </div>
        </div>
      </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'AppHeader',
  props: ["datimyNav"],
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';
img{
  width:40%;
}

li{
  list-style-type: none;
  display: inline;
  padding: 14px;
  color: $daisy;
  a{
    color: $daisy;
    text-decoration: none;
  }
}
h1{
  color: $daisy;
}
p{
  color: $mamba;
}
.header-bg{
  padding-top: 100px;
}
</style>
