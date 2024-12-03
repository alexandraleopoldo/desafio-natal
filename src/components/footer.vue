<script setup>
import face from "../assets/logo-facebook.png"
import google from "../assets/logo-google.png"
import insta from "../assets/logo-instagram.png"
import tw from "../assets/logo-twitter.png"
import whats from "../assets/logo-whatsapp.png"
import logo from "../assets/logo.png"
</script>

<template>
    <footer>
        <img :src="logo" alt="Logo: Feliz Natal" class="logo-footer">
        <div>
           <a href="https://x.com/crian_esperanca" target="_blank"> <img :src="tw" alt="Logo Twitter"></a>

            <a href="https://api.whatsapp.com/send?text=https%3A%2F%2Fredeglobo.globo.com%2Fcriancaesperanca%2Fnoticia%2Ffale-com-a-glo-no-zap-e-acesse-conteudos-exclusivos-do-crianca-esperanca.ghtml%3Futm_source%3Dwhatsapp%26utm_medium%3Dshare-bar-desktop%26utm_campaign%3Dmaterias" target="_blank"><img :src="whats" alt="Logo Whatsapp"></a>

            <a href="https://www.instagram.com/crianca.esperanca/" target="_blank"><img :src="insta" alt="Logo Instagram"></a>

            <a href="https://www.facebook.com/tvglobo/videos/crian%C3%A7a-esperan%C3%A7a-2023-a-campanha-t%C3%A1-no-ar/1740262043075415/" target="_blank"><img :src="face" alt="Logo Facebook"></a>

           <a href="https://redeglobo.globo.com/criancaesperanca/" target="_blank"> <img :src="google" alt="Logo Google"></a>
        </div>
    </footer>
</template>

<style scoped lang="scss">
 footer {
    display: flex;
    align-items: center;
    height: 60px;
    justify-content: space-around;
    background-color:  #FFE9E8;
 }

 .logo-footer {
    width: 120px;
    height: 30px;
 }

 div {
    display: flex;
    align-items: center;
    gap: 20px;
    img {
        width: 30px;
    }
 }
</style>