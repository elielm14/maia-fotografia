<template>
  <div class="main">
    <h1>{{ tituloPag }}</h1>
    <div class="fotos-api">
      <ul class="lista-api">
        <li class="item-api" v-for="imagem in imagens" :key="imagem.id">

          <a :href="imagem.url">

            <img :src="imagem.src.portrait" :alt="imagem.titulo">

          </a>

        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import { createClient } from 'pexels';

export default {

  data(){
      
    return{
      tituloPag: 'Photos On',
      imagens:[]
    }
  },

  async created(){

    try {
      const client = createClient('563492ad6f91700001000001e6d8a5315f0240f3902236ca5b3fb1b5');
      const query = 'pessoas';
      client.photos.search({ query, locale: 'pt-BR'/* , page: 2  */}).then(response => {
        this.imagens = response.photos
      });

    } catch (error) {
      console.log(error)
    }
  },

  methods:{
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