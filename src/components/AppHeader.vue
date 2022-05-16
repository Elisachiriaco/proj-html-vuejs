<template>
    <div class="container">
      <div class="row align-items-center">
        <div class="col-4 justify-content-start">
          <img src="../assets/images/avada-bakery-logo-retina.png" alt="logo">
        </div>
        <div class="col-8 justify-content-end">
        <ul>
          <li><a href="#">{{myArray[0].nome}}</a></li>
          <li><a href="#">{{myArray[1].nome}}</a></li>
          <li><a href="#">{{myArray[2].nome}}</a></li>
          <li><a href="#">{{myArray[3].nome}}</a></li>
          <li><a href="#">{{myArray[4].nome}}</a></li>
          <li><a href="#">{{myArray[5].nome}}</a></li>
          <li><a href="#">{{myArray[6].nome}}</a></li>
          <li><a href="#">{{myArray[7].nome}}</a></li>
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
import dati from '../dati.json'
export default {
  name: 'AppHeader',
  data(){
    return{
      myArray: dati,
    }
  }
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
