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

<!--       <p class="texto-divulgação">"Toda história de amor é bonita, mas as que contamos são as nossas favoritas!". Eliel Maia, 2021.</p> -->

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
  color: #6e0d0d;
  padding: 0px;
  width: auto;
  margin: 0 auto;
}
.caixa{
  padding: 50px;
  background-image: url(https://images.pexels.com/photos/5389414/pexels-photo-5389414.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=500&w=500);
  height: 200px;
  background-attachment: fixed;
  background-position-x: 0px;
  background-position-y: -300px;
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
  color: #333333;;
  font-weight: 600;
  margin-top: 5px;
  text-decoration: none;
  font-family: Arial, Helvetica, sans-serif;
}
#nav a.router-link-exact-active {
  color: #000000;
}
@media (min-width: 50px)and (max-width: 150px){
  .caixa{
    padding: 1px;
    height: 320px;
    background-image: none;
}
h1{
  margin-top: 0;
  text-align: center;
  font-size: 20px;
}
#nav{
  text-align: center;
}
#nav a{
  font-size: 15px;
  padding: 0px 10px;
}
ul{
  margin: 0;
  padding: 0;
}
.caixa{
  height: 40%;
}
}
@media (min-width: 151px)and (max-width: 205px){
  .caixa{
    padding: 1px;
    height: 320px;
    background-image: none;
}
h1{
  margin-top: 0;
  text-align: center;
  font-size: 20px;
}
#nav{
  text-align: center;
}
#nav a{
  font-size: 15px;
  padding: 0px 10px;
}
ul{
  margin: 0;
  padding: 0;
}
.caixa{
  height: 40%;
}
}
@media (min-width: 206px)and (max-width: 279px){
  .caixa{
    padding: 1px 20px;
    height: 320px;
    background-attachment: fixed;
    background-position-x: -277px;
    background-position-y: -21px;
}
h1{
  margin-top: 0;
}
#nav{
  text-align: center;
}
#nav a{
  font-size: 25px;
  padding: 0px 10px;
}
ul{
  margin: 0;
  padding: 0;
}
}
@media (min-width: 280px)and (max-width: 319px){
  .caixa{
    padding: 1px 20px;
    height: 320px;
    background-attachment: fixed;
    background-position-x: -277px;
    background-position-y: -21px;
}
h1{
  margin-top: 0;
}
#nav{
  text-align: center;
}
#nav a{
  font-size: 25px;
  padding: 0px 10px;
}
ul{
  margin: 0;
  padding: 0;
}
}
@media (min-width: 320px)and (max-width: 480px){
  .caixa{
    padding: 1px;
    height: 320px;
    background-attachment: fixed;
    background-position-x: -277px;
    background-position-y: -21px;
}
h1{
  margin-top: 0;
}
#nav{
  text-align: center;
}
#nav a{
  font-size: 25px;
  padding: 0px 10px;
}
ul{
  margin: 0;
  padding: 0;
}
}
@media (min-width: 481px)and (max-width: 520px){
  .caixa{
    padding: 1px;
    height: 320px;
    background-attachment: fixed;
    background-position-x: -230px;
    background-position-y: -21px;
}
h1{
  margin-top: 0;
}
#nav{
  text-align: center;
}
#nav a{
  font-size: 25px;
  padding: 0px 10px;
}
ul{
  margin: 0;
  padding: 0;
}
}
@media (min-width: 521px)and (max-width: 600px){
  .caixa{
    padding: 1px;
    height: 320px;
    background-attachment: fixed;
    background-position-x: -217px;
    background-position-y: -22px;
}
h1{
  margin-top: 0;
}
#nav{
  text-align: center;
}
#nav a{
  font-size: 25px;
  padding: 0px 10px;
}
ul{
  margin: 0;
  padding: 0;
}
}
@media (min-width: 600px)and (max-width: 780px){
  .caixa{
    padding: 1px;
    height: 320px;
    background-attachment: fixed;
    background-position-x: -166px;
    background-position-y: -22px;
}
h1{
  margin-top: 0;
}
#nav{
  text-align: center;
}
#nav a{
  font-size: 25px;
  padding: 0px 10px;
}
ul{
  margin: 0;
  padding: 0;
}
}
@media (min-width: 781px)and (max-width: 899px){
  #nav {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: right;
  color: #6e0d0d;
  padding: 0px;
  width: auto;
  margin: 0 auto;
}
.caixa{
  padding: 50px;
  background-image: url(https://images.pexels.com/photos/5389414/pexels-photo-5389414.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=500&w=500);
  height: 200px;
  background-attachment: fixed;
  background-position-x: -186px;
  background-position-y: -206px;
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
  color: #333333;;
  font-weight: 600;
  margin-top: 5px;
  text-decoration: none;
  font-family: Arial, Helvetica, sans-serif;
}
#nav a.router-link-exact-active {
  color: #000000;
}
}
@media (min-width: 1450px)and (max-width: 2560px){
  #nav {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: right;
  color: #6e0d0d;
  padding: 0px;
  width: auto;
  margin: 0 auto;
}
.caixa{
  padding: 50px;
  background-image: url(https://images.pexels.com/photos/5389414/pexels-photo-5389414.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=500&w=500);
  height: 450px;
  background-attachment: fixed;
  background-position-x: -469px;
  background-position-y: -632px;
  background-repeat: no-repeat;
  background-size: cover;
}
h1{
  font-size: 60px;
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
  font-size: 35px;
  padding: 10px 15px;
  color: #333333;;
  font-weight: 600;
  margin-top: 5px;
  text-decoration: none;
  font-family: Arial, Helvetica, sans-serif;
}
#nav a.router-link-exact-active {
  color: #000000;
}
}
</style>