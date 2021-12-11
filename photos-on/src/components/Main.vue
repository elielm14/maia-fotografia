<template>
  <div class="main">

    <ul>

      <li class="lista-fotos-item" v-for="imagem in imagens" :key="imagem.id">

      <!--   <img :src="imagem.src.landscape" :alt="imagem.titulo"> -->

        <progressive-img :src="imagem.src.landscape" :placeholder="imagem.src.small" :blur="30"/>

      </li>

    </ul>

    <button v-on:click="paginaAnterior" class="botao">Página Anterior</button>
    <button v-on:click="proximaPagina" class="botao">Proxima página</button>

  </div>

</template>

<script>
import { createClient } from 'pexels';

export default {

  data(){
      
    return{

      imagens:[],
      pagina: 1
    }
  },

  async created(){
    await this.carregaPagina()
  },

  methods:{
        proximaPagina: function(){
        this.pagina = this.pagina + 1
        console.log(this.pagina);
        this.carregaPagina()
    },
    paginaAnterior: function(){
        this.pagina = this.pagina - 1
        console.log(this.pagina);
        this.carregaPagina()
    },

    async carregaPagina(){
    try {
      const client = createClient('563492ad6f91700001000001e6d8a5315f0240f3902236ca5b3fb1b5');
      const query = 'casamento';
      client.photos.search({ query, locale: 'pt-BR', per_page: 8, page: [this.pagina] }).then(response => {
        this.imagens = response.photos
      });

    } catch (error) {
      console.log(error)
    }
    }
  }
}
</script>

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
.botao{
    width: 15%;
    padding: 15px 0;
    margin: 30px 0 0 30px;
    background: #6e0d0d;;
    color: white;
    font-weight: bold;
    font-size: 18px;
    border: none;
    border-radius: 5px;
    transition: 1s;
    cursor: pointer; 
}
.botao:hover{
    transform: scale(1.2);
}
</style>