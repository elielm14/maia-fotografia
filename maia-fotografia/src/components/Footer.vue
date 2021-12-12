<template>

    <footer class="footer-fundo">

        <p class="copyrigth">&copy; Copyrigth Maia fotografia 2021</p>

        <section>

            <ul>

                <li>
                    <a href="https://www.instagram.com/" target="_blank" class="logo-contato">
                    <img src="https://cdn-icons-png.flaticon.com/512/2111/2111491.png" alt="instagram"></a>
                </li>

                <li>
                    <a href="https://api.whatsapp.com/send?phone=5591986060649&text=sua%20mensagem" target="_blank" class="logo-contato">
                    <img src="https://cdn-icons-png.flaticon.com/512/1384/1384023.png" alt="whatsapp"></a>
                </li>

            </ul>

      </section>

    </footer>

</template>

<style scoped>
footer{
    text-align: center;
}
.copyrigth{
    color: #000000;
    font-size: 15px;
    margin-left: auto;
}
ul{
    margin-top: 20px;
    margin-left: auto;
    padding: 0px;
}
li{
    display: contents;
}
a{
    text-decoration: none;
}
a:-webkit-any-link{
    cursor: pointer;
    color: black;
}
img{
    width: 30px;
    padding: 0px 5px 0px 0px;
}
@media (min-width: 1450px)and (max-width: 2808px){
.copyrigth{
    color: #000000;
    font-size: 30px;
    margin-left: auto;
}
img{
    width: 50px;
    padding: 0px 5px 0px 0px;
}
}
</style>