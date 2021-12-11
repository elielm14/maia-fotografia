<template>
    <div>
        <section class="pricipal">
            <h1>Maia Fotografia</h1>
            <img class = "recepcao" src="https://images.pexels.com/photos/3771110/pexels-photo-3771110.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940" alt="foto-recepcao">
            <p>Somos o portal líder em fotografia de casamentos: somos românticos que ajudam casais apaixonados nos registros do grande dia. Um momento único para aproveitar com a família e os amigos precisa ser guardado para sempre.

            <p>Nos divertimos compartilhando experiências com milhares de noivas e noivos, nos emocionamos com suas histórias. Fazemos tudo isso com a colaboração de muitos profissionais da área dotados de conhecimentos técnicos, criatividade e experiência.</p>
        </section>

        <section class="beneficios">
            
            <h2>Somos referência em fotografia</h2>

            <div class="caixa-beneficio">

                <div class="caixa-foto"><img class="fotografo" src="https://images.pexels.com/photos/1406374/pexels-photo-1406374.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940" alt="fotografo"></div>

                <ul>

                    <li class="item">Atendimento personalizado.</li>
                    <li class="item">Pacotes com cerimonialista(o) incluso.</li>
                    <li class="item">Especialista em fotos externas e internas.</li>
                    <li class="item">Parcerias com os melhores buffet da região.</li>

                </ul>

            </div>

        </section>

        <section class="mapa">

            <h3>Nosso estabelecimento</h3>

            <p class="mapa-texto">Nossa empresa esta localizada no coração da cidade</p>

            <div class="mapa-conteudo"><iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3988.6023882719105!2d-48.476929985898146!3d-1.4145775361769493!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x92a48bde151b7e13%3A0x885190cc122ea971!2sPassagem%20Severa%20Romana%20-%20Sacramenta%2C%20Bel%C3%A9m%20-%20PA%2C%2068447-000!5e0!3m2!1spt-BR!2sbr!4v1638993857323!5m2!1spt-BR!2sbr" width="100%" height="300" style="border:0;" allowfullscreen="" loading="lazy"></iframe></div>

        </section>

    </div>

</template>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Oswald&family=Playfair+Display:ital,wght@1,500&display=swap');

.pricipal, .mapa, .beneficios{
    margin: 100px 0 10px 0;
}
h1 ,h2, h3{
    text-align: center;
    margin: 15px 0px 20px 0px;
    font-family: 'Oswald', sans-serif;
    font-family: 'Playfair Display', serif;
    font-size: 40px;
}
p{
    text-align: justify;
    margin: 0px 15px 0px 15px;
    padding: 8px 0;
    font-size: 20px;
}
.recepcao{
width: 250px;
padding: 0 20px 0 20px;
float: left;
}
.mapa-texto{
    text-align: center;
    margin: 20px 0;
}
.caixa-foto{
   padding: 30px 0 0 0;
}
.fotografo{
    width: 200px;
    padding: 9px 20px 0 20px;
    float: left;
    margin: 0 0 0 30%;
}
ul{
    margin: 50px 0px 150px 0px;
}
li{
    font-size: 20px;
}
.item{
    line-height: 1.5;
    list-style: none;
}
.item:before{
    content: "❤️";
    margin: 0 8px 0 0;
}
</style>