<template>
  <div class="main">

    <ul>

      <li class="lista-fotos-item" v-for="imagem in imagens" :key="imagem.id">

      <!--   <img :src="imagem.src.landscape" :alt="imagem.titulo"> -->

        <progressive-img :src="imagem.src.landscape" :placeholder="imagem.src.small" :blur="30" />

      </li>

    </ul>

  </div>

</template>

<script>
import { createClient } from 'pexels';

export default {

  data(){
      
    return{

      imagens:[],
      pagina: [1]
    }
  },

  async created(){

    try {
      const client = createClient('563492ad6f91700001000001e6d8a5315f0240f3902236ca5b3fb1b5');
      const query = 'casamento';
      client.photos.search({ query, locale: 'pt-BR', per_page: 8, page: this.pagina }).then(response => {
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
li{
  list-style: none;
}
.lista-fotos-item{
  padding: 40px 0px;
}
.progressive-image{
width: 800px;
height: auto;
}
</style>