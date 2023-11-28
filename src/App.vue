<template>
  <div class="background-figure left"><img src="./assets/background/Vector.svg" alt="" srcset=""></div>
  <div class="background-figure right"><img src="./assets/background/Vector_right.svg" alt="" srcset=""></div>
  <HeaderComponent />
  <HomePage />
  <FooterComponent class="footer-component" />
</template>

<script>
import HomePage from './Pages/HomePage.vue'
import HeaderComponent from './components/Header.vue'
import FooterComponent from './components/Footer.vue'
export default {
  name: 'App',
  components: {
    HomePage,
    HeaderComponent,
    FooterComponent
  }
}
</script>

<style>
* {
  padding: 0px;
  margin: 0px;
}

#app {
  margin-top: 30px;
}

.footer-component {
  margin-top: 180px;
}

.background-figure {
  position: absolute;
  z-index: -1;
}

.left {
  top: -30px;
}

.right {
  top: 300px;
  right: 0px;
}
</style>
