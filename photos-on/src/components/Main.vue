<template>
  <div class="main">
    <h1>{{ tituloPag }}</h1>
    <div class="fotos-api">
      <ul class="lista-api">
        <li class="item-api" v-for="fotos in fotos" :key="fotos.url">
          <img :src="fotos.url" :alt="fotos.titulo">
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import { createClient } from 'pexels';

const client = createClient('563492ad6f91700001000001e6d8a5315f0240f3902236ca5b3fb1b5');
const query = 'Nature';
client.photos.search({ query }).then(photos => console.log(photos));

export default {

  data(){
      
    return{
      tituloPag: 'Photos On',
      photos:[]
    }
  },
}
</script>

<!-- scoped para uso de estilo exclusivo -->
<style scoped>
.fotos-api .lista-api{
  display: inline;
  width: 350px;
  height: 350px;
}
.item-api{
  height: 320px;
  max-width: 320px;
  vertical-align: bottom;
  padding: 20px;
}
</style>