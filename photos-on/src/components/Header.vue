<template>
<div id="nav">

  <h1>Photos On</h1>

      <router-link to="/" class="nav-menu">Início</router-link> |

      <router-link to="/about" class="nav-menu">Sobre nós</router-link> |

      <router-link to="/contact" class="nav-menu">Contato</router-link>

      <p class="texto-divulgação">"Toda história de amor é bonita, mas a que contamos é a minha favorita!". Eliel Maia, 2021.</p>

</div>

</template>

<script>

</script>


<style scoped>
#nav {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: right;
  color: #000000;
  padding: 50px;
  width: auto;
  margin: 0 auto;
  background-image: url(https://images.pexels.com/photos/45960/pexels-photo-45960.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940);
  min-height: 350px;
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
h1{
  font-size: 40px;
  padding: 10px;
  font-weight: 750;
  margin-right: 15px;
}
#nav a {
  font-size: 25px;
  padding: 10px;
  color: #000000;;
  font-weight: 600;
  margin-top: 5px;
  margin-right: 15px;
}
#nav a.router-link-exact-active {
  color: #3a499e;
}
.texto-divulgação{
  text-align: center;
  margin: 120px 0 0 0;
  font-size: 25px;
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}
</style>