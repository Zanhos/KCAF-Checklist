<template>
  
  <div id="app">
    <Header></Header>
    <Banner></Banner>
    <Home></Home>
    <!-- <Documents></Documents> -->
    <!-- <Newsletter></Newsletter> -->
    <Footer></Footer>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Banner from './components/Banner.vue';
import Home from './components/Home.vue';
// import Documents from './components/Documents.vue';
// import Newsletter from './components/Newsletter.vue';
import Footer from './components/Footer.vue'

export default {
  name: 'app',
  components: {
    Header,
    Banner,
    Home,
    // Documents,
    // Newsletter,
    Footer,
  }
}
</script>

<style lang="scss">
  @import 'assets/sass/extends.scss';

  html {
      box-sizing: border-box;
      font-family: $main-font, 'Helvetica Neue', 'Arial', 'Lato';
      text-shadow: 0 1px 0 rgba(0, 0, 0, 0.07);
      scroll-behavior: smooth;
  }

  [v-cloak] { display: none; }
  
  *, *:before, *:after { box-sizing: inherit; }

  h1 { font-size: 1.6rem; }
  h2 { font-size: 1.4rem; }
  h3 { font-size: 1.2rem; }
  h4 { font-size: 1.0rem; }

  body {
      margin: 0;
  }

  img[alt="logo"] {
      width: 2.7rem;
      margin-top: -0.4rem;
  }

  @import 'assets/sass/media_queries.scss';
</style>
