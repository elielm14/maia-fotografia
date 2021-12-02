<template>
  <div id="app">
    <div id="nav">
      <router-link to="/" class="nav-menu">Home</router-link> |
      <router-link to="/about" class="nav-menu">About</router-link> |
      <router-link to="/contact" class="nav-menu">Contact</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
}

#nav {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: right;
  color: #000000;
  padding: 30px;
}

#nav a {
  font-size: 20px;
  padding: 8px;
  color: #000000;
}
/* estilo do link ativo no momento */
#nav a.router-link-exact-active {
  color: #031cad;
}
</style>