<template>
<div id="nav">

  <h1>Photos On</h1>

      <router-link to="/" class="nav-menu">Início</router-link> |

      <router-link to="/about" class="nav-menu">Sobre nós</router-link> |

      <router-link to="/contact" class="nav-menu">Contato</router-link>

</div>

</template>

<script>

</script>


<style scoped>
#nav {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: right;
  color: #ffffff;
  padding: 50px;
  width: auto;
  margin: 0 auto;
  background-image: url(https://images.pexels.com/photos/261763/pexels-photo-261763.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940);
  min-height: 350px;
  background-attachment: fixed;
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
  opacity: 0.9;
}
h1{
  font-size: 40px;
  padding: 10px;
  font-weight: bold;
  margin-right: 15px;
}
#nav a {
  font-size: 25px;
  padding: 10px;
  color: #ffffff;;
  font-weight: 500;
  margin-right: 15px;
}
#nav a.router-link-exact-active {
  color: #001797;
}
</style>