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

export default {

  data(){
      
      return{
        tituloPag: 'Photos On',
        fotos:[
          {
            url: 'https://media.gazetadopovo.com.br/viver-bem/2018/11/dog3-600x459-0e01be20.jpg',
            titulo: 'cachorro preto'
          },
          {
            url: 'https://blog.appegada.com/thumb/blog/1/780/500/1a09bacc2740e0f8e3c2b10bd5bf01ae.jpg',
            titulo: 'cachorro caramelo'
          }
        ]
      }
    },

    created(){
      let promise = this.$http.get('http://api.pexels.com/v1/');
      promise.then(res => res.json()
      .then())
    }
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