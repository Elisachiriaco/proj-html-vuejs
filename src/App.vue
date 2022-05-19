<template>
  <div id="app">
    <header>
    <app-header :datimyNav = "datimyNav" />
    </header>
    <main>
      <app-main :datimySlider = "datimySlider" :datiSecondSlider = "datiSecondSlider" />
    </main>
    <footer>
      <app-footer :datimyFooter = "datimyFooter" :datiCopyright = "datiCopyright"/>
    </footer>
  </div>
</template>

<script>
import AOS from "aos";
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
import dati from './dati.js'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter
  },
  data(){
    return{
      datimyNav : dati.myNav,
      datimyFooter : dati.myFooter,
      datiCopyright : dati.copyright,
      datimySlider : dati.slider,
      datiSecondSlider : dati.secondSlider
    };
  },
    created(){
      AOS.init();
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
  position: relative;
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
  transition: all 0.5s;
  a{
    text-decoration: none;
    color: $daisy;
    font-size: 14px;
  }
  &:hover{
    background-color: $daisy;
    a{
      color: $white;
    }
  }
}
.mybutton-violet{
  background-color: $daisy;
  width: 150px;
  height: 35px;
  border-radius: 4px;
  line-height: 35px;
  transition: all 0.5s;
  a{
    text-decoration: none;
    color: $white;
    font-size: 14px;
  }
  &:hover{
    background-color: $white;
    border: 2px solid rgba($color: $daisy, $alpha: 0.2);
    a{
      color: $daisy;
    }
  }
}
h3{
    color: $daisy;
    padding-bottom: 15px;
}
h2{
  color: $white;
  font-size: 40px;
}
</style>
