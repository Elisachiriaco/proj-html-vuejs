<template>
    <div class="container">
      <div class="row align-items-center">
        <div class="col-4 justify-content-start">
          <img src="../assets/images/avada-bakery-logo-retina.png" alt="logo">
        </div>
        <div class="col-8 justify-content-end">
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">Shop</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Gallery</a></li>
          <li><a href="#">Locations</a></li>
          <li><a href="#">Journal</a></li>
          <li><a href="#">Contact</a></li>
          <li><a href="#">My Account</a></li>
          <li><a href="#"><i class="fa-solid fa-cart-shopping"></i></a></li>
        </ul>
      </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'AppHeader',
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
  padding: 10px;
  a{
    color: $daisy;
    text-decoration: none;
  }
}
</style>
