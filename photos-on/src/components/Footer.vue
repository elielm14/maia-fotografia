<template>

    <footer class="footer-fundo">

        <p class="copyrigth">&copy; Copyrigth Photos On 2021</p>

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
/* .footer-fundo{
    background-image: url(https://images.pexels.com/photos/1303092/pexels-photo-1303092.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940);
    height: 100px;
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;

} */
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
</style>