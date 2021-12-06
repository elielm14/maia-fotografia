<template>

    <footer class="footer-fundo">

        <p class="copyrigth">&copy; Copyrigth Photos On 2021</p>

        <section>

            <ul>

                <li>
                    <a href="https://www.instagram.com/" target="_blank" class="logo-contato">
                    <img src="https://cdn-icons-png.flaticon.com/512/2111/2111491.png" alt="instagram">Maia Fotografia</a>
                </li>

                <li>
                    <a href="https://api.whatsapp.com/send?phone=5591986060649&text=sua%20mensagem" target="_blank" class="logo-contato">
                    <img src="https://cdn-icons-png.flaticon.com/512/1384/1384023.png" alt="whatsapp">Maia Fotografia</a>
                </li>

            </ul>

      </section>

    </footer>

</template>

<style scoped>
footer{
    padding: 40px 0;
    text-align: center;
}
.copyrigth{
    color: #000000;
    font-size: 20px;
    margin-top: 150px;
    }
.footer-fundo{
    background-image: url(https://images.pexels.com/photos/261763/pexels-photo-261763.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940);
    min-height: 300px;
    background-attachment: fixed;
    background-position: bottom;
    background-repeat: no-repeat;
    background-size: cover;
}
ul{
    margin-top: 20px;
}
li{
    display: block;
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
    padding: 15px 15px 0px 0px;
}
</style>