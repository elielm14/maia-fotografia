<template>
  <div class="home">

    <Header/>

    <Main/>

    <Footer/>

  </div>
</template>

<script>
//import dos componentes
import Main from '../components/Main.vue'
import Header from '../components/Header.vue'
import Footer from '../components/Footer.vue'

export default {
  name: 'Home',
  components: {
    Main,
    Header,
    Footer
  }
}
</script>
