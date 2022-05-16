<template>
  <div id="app">
    <header>
    <app-header />
    </header>
    <main>
      <app-main />
    </main>
    <footer>
      <app-footer />
    </footer>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter
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
  font-size: 12px;
  padding-bottom: 5px;
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
    font-size: 10px;
  }
}
.mybutton-violet{
  background-color: $daisy;
  width: 150px;
  height: 35px;
  border-radius: 4px;
  line-height: 35px;
  a{
    text-decoration: none;
    color: $white;
    font-size: 12px;
  }
}
</style>
