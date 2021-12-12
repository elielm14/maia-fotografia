<template>

    <main>

        <form>

            <label for="Nome e Sobrenome">Nome e Sobrenome</label>
            <input type="text" name="nomeSobrenome" id="nomeSobrenome" placeholder="Nome e Sobrenome" required>

            <label for="E-mail">E-mail</label>
            <input type="email" name="email" id="email" placeholder="seuemail@dominio.com.br">

            <label for="telefone" >Telefone</label>
            <input type="tel" name="telefone" id="telefone" placeholder="(xx) xxxxx-xxxx" required>

            <label for="mensagem">Mensagem</label>
            <textarea name="mensagem" id="mensagem" cols="70" rows="10" class="input-padrao" required placeholder="Deixe sua mensagem"></textarea>

        </form>

        <fieldset>
                
                <legend>Como prefere o nosso contato?</legend>

                 <label for="radio-email"><input type="radio" name="contato" id="radio-email" value="email">Email</label>
                
                 <label for="radio-telefone"><input type="radio" name="contato" id="radio-telefone" value="telefone">Telefone</label>
                
                 <label for="radio-what"><input type="radio" name="contato" id="radio-what" value="what" checked >WhatsApp</label>
                
        </fieldset>

        <input type="submit" value="Enviar formulário" class="enviar">

    </main>

</template>

<style scoped>
main{
    margin: 40px 70px;
    font-size: 20px;
    font-family: Arial, Helvetica, sans-serif;
}
form{
    display: grid;
    margin: 0 0 10px 30px;
    padding: 10px 0;
}
#nomeSobrenome, #email, #telefone, #mensagem{
    margin: 0 0 10px;
    padding: 10px 20px;
    width: 50%;
}
fieldset{
    width: 50%;
    display: grid;
    padding: 10px 0;
    margin: 0 0 30px 30px;
}
.enviar{
    width: 40%;
    padding: 15px 0;
    margin: 0 0 0 30px;
    background: #6e0d0d;;
    color: white;
    font-weight: bold;
    font-size: 18px;
    border: none;
    border-radius: 5px;
    transition: 1s;
    cursor: pointer; 
}
.enviar:hover{
    transform: scale(1.2);
}
label{
    padding: 5px 0;
}
::placeholder{
    font-size: 18px;
    text-align: justify;
    font-family: Arial, Helvetica, sans-serif;
}
@media (min-width: 320px)and (max-width: 520px){
main{
    margin: 21px 20px;
    font-size: 20px;
}
form{
    margin: 0 0 0px 15px;
    padding: 0px 0;
}
#nomeSobrenome, #email, #telefone, #mensagem{
    margin: 15px 0 15px;
    width: 80%;
}
fieldset{
    width: 80%;
    padding: 5px 0;
    margin: 15px 15px 15px 15px;
}
.enviar{
    width: 50%;
}
}
</style>