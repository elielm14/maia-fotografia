<template>
  <div class="home">
    <img alt="cachorro na caneca" src="https://blog.emania.com.br/wp-content/uploads/2019/01/como-tirar-foto-de-cachorro.jpg">
    <img src="https://www.dicaspetz.com.br/wp-content/uploads/2019/06/cachorro-filhote.jpg" alt="cachorro branco">
    <img src="https://matsudapet.com.br/blog/wp-content/uploads/2019/08/shutterstock_559799125-compressed.jpg" alt="cachorro branco rindo">
    <img src="https://media.gazetadopovo.com.br/viver-bem/2018/11/dog3-600x459-0e01be20.jpg" alt="cachorro preto">
    <Main/>
  </div>
</template>

<script>
//import do componete principal
import Main from '../components/Main.vue'

export default {
  name: 'Home',
  components: {
    Main
  }
}
</script>
