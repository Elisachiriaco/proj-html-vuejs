<template>
    <div class="container" id="home">
      <div class="row align-items-center">
        <div class="col-4 justify-content-start">
          <img src="../assets/images/avada-bakery-logo-retina.png" alt="logo">
        </div>
        <div class="col-8 justify-content-end">
        <ul>
          <li v-for="(item, index) in datimyNav" :key="index" :class="{'active' : index === activeIndex}" @click="activeIndex = index">
            <a :href="item.link">{{item.nome}}</a>
          </li>
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
      <div class="row">
        <div class="col-12">
        <div class="prebuilts">
          <a href="#"> <i class="fa-solid fa-folder-open"></i> <br> Prebuilts</a>
        </div>
        </div>
      </div>
      <div class="row">
        <div class="col">
        <div class="buy">
          <a href="#"><i class="fa-solid fa-cart-shopping fa-bounce"></i> 
          <br> Buy Now</a>
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
  data(){
    return{
      activeIndex : 0
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
  color: $daisy;
  cursor: pointer;
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
.active{
  border-bottom: 2px solid $daisy;
}


.prebuilts{
  position: fixed;
  top: 200px;
  right: 10px;
  width: 70px;
  height: 70px;
  background-color: $white;
  border-radius: 10px;
  z-index: 2000;
  box-shadow: 2px 2px #888888;
  cursor: pointer;
  text-align: center;
  i{
    font-size: 20px;
    color: $limed;
    padding-top: 10px;
  }
  a{
    color: $limed;
    text-decoration: none;
    font-size: 10px;
  }
}

.buy{
  position: fixed;
  top: 120px;
  right: 10px;
  width: 70px;
  height: 70px;
  background-color: $white;
  border-radius: 10px;
  z-index: 2000;
  box-shadow: 2px 2px #888888;
  cursor: pointer;
  text-align: center;
  i{
    font-size: 20px;
    color: $limed;
    padding-top: 10px;
  }
  a{
    color: $limed;
    text-decoration: none;
    font-size: 10px;
  }
}
</style>
