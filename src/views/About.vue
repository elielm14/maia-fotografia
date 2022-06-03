<template>
  <div class="about">
    <Header/>

    <Historia/>

    <Footer/>
  </div>
</template>

<script>
import Header from '../components/Header.vue'
import Footer from '../components/Footer.vue'
import Historia from '../components/Historia.vue'

export default {
  name: 'About',
  components: {
    Header,
    Footer,
    Historia
  }
}
</script>
