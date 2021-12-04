<template>
  <div class="main">

    <div class="fotos-api">

      <ul class="lista-fotos">

        <li class="lista-fotos-item" v-for="imagem in imagens" :key="imagem.id">

          <img :src="imagem.src.medium" :alt="imagem.titulo">

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
.main{
text-align: center;
}
.lista-fotos .lista-fotos-item{
  display: inline-block;
}
.lista-fotos-item{
  height: auto;
  width: 100%;
  list-style: none;
  padding: 10px 0px;
}
</style>