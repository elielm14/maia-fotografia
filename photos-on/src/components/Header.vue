<template>
<div id="nav">

  <header>

    <div class="caixa">
      
      <h1>Maia Fotografia</h1>

        <nav>

          <ul>

          <li><router-link to="/" class="nav-menu">Início</router-link>|</li>
          <li><router-link to="/about" class="nav-menu">Sobre nós</router-link>|</li>
          <li><router-link to="/contact" class="nav-menu">Contato</router-link></li>

          </ul>

        </nav>

      <p class="texto-divulgação">"Toda história de amor é bonita, mas a que contamos é a minha favorita!". Eliel Maia, 2021.</p>

    </div>

  </header>

</div>

</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Oswald&family=Playfair+Display:ital,wght@1,500&display=swap');
#nav {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: right;
  color: #000000;
  padding: 0px;
  width: auto;
  margin: 0 auto;
}
.caixa{
  padding: 50px;
  background-image: url(https://images.pexels.com/photos/45960/pexels-photo-45960.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940);
  min-height: 380px;
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
  font-family: 'Oswald', sans-serif;
  font-family: 'Playfair Display', serif;
}
li{
  display: contents;
}
#nav a {
  font-size: 25px;
  padding: 10px 15px;
  color: #000000;;
  font-weight: 600;
  margin-top: 5px;
  text-decoration: none;
  font-family: Arial, Helvetica, sans-serif;
}
#nav a.router-link-exact-active {
  color: #2c366b;
}
.texto-divulgação{
  text-align: center;
  margin: 120px 0 0 0;
  font-size: 25px;
  font-family: Arial, Helvetica, sans-serif;
}
</style>