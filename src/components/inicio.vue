<script setup>
import loja from "../assets/loja.png"
import logo from "../assets/logo.png"
</script>

<template>
    <section>
        <div class="texto-inicio">
            <img :src="logo" alt="">
            <h1>Uma 
                <span>plataforma de doação</span>
            para espalhar alegria</h1>
            <p>Nessas festas de fim de ano mande um presente para a pessoa amada e compartilhe a alegria do Natal.</p>
            <a href="https://doacoes.criancaesperanca.unesco.org/" target="_blank"><button>FAZER UMA DOAÇÃO</button></a>

        </div>
        <div class="image">
            <img :src="loja" alt="">
        </div>
    </section>
</template>

<style scoped lang="scss">
 section {
    display: flex;
    align-items: center;
    background-color: #FFE9E8;
    height: 420px;
    justify-content: space-evenly;
 }

.texto-inicio {
    display: flex;
    flex-direction: column;
    width: 35%;
    padding: 30px;
    justify-self: end;
    background-color: brown;
    gap: 20px;
}

 .image {
    width: 45%;
    background-color: aqua;
    
   img{
    width: 60%;
   }
    
 }
</style>