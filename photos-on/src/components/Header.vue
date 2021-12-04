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
h1{
  font-size: 40px;
  padding: 10px;
  font-weight: 600;
}
#nav {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: right;
  color: #000000;
  padding: 30px;
  font-weight: 300;
}

#nav a {
  font-size: 25px;
  padding: 10px;
  color: #000000;
}
/* estilo do link ativo no momento */
#nav a.router-link-exact-active {
  color: #031cad;
}
</style>