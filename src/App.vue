<template>
  <div id="app">
    <header>
    <AppHeader />
    </header>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'

export default {
  name: 'App',
  components: {
    AppHeader
  }
}
</script>

<style lang="scss">
@import "./style/generals.scss";
@import "./style/vars.scss";

header{
  background-image: url(./assets/images/hero-header-bakery.jpg);
  background-size: cover;
  width: 100%;
  height: 600px;
}
.subtitle{
  text-transform: uppercase;
  color: $mamba;
}
.mybutton-white{
  background-color: $white;
  width: 150px;
  height: 35px;
  border-radius: 4px;
  line-height: 35px;
  a{
    text-decoration: none;
    color: $daisy;
    font-size: 12px;
  }
  }
</style>
