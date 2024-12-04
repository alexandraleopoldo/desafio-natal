<script setup>
import loja from "../assets/loja.png"
import logo from "../assets/logo.png"

const doacao = () => {
  window.open("https://doacoes.criancaesperanca.unesco.org/", "_blank");
};

</script>

<template>
    <section>
        <div class="texto-inicio">
            <img :src="logo" alt="">
            <h1>Uma 
                <span>plataforma de doação</span>
            para espalhar alegria</h1>
            <p>Nessas festas de fim de ano mande um presente para a pessoa amada e compartilhe a alegria do Natal.</p>
            <button @click="doacao" class="estilo-button">FAZER UMA DOAÇÃO</button>


        </div>
        <div class="image">
            <img :src="loja" alt="">
        </div>
    </section>
</template>

<style scoped lang="scss">
 section {
    width: 100%;
    display: flex;
    align-items: center;
    background-color: #FFE9E8;
    height: 420px;
    justify-content: space-evenly;
 }

.texto-inicio {
    display: flex;
    flex-direction: column;
    width: 30%;
    padding: 30px;
    justify-self: end;
    gap: 20px;

    img {
        width: 20%;
    }

    h1 {
        font-size: 34px;
    }

    p {
          width: 80%;
          line-height: 30px;
          font-size: 16px;
          font-weight: 400;
        }

    span {
        color:  #CD3C32;
        
    }
}

 .image {
    width: 40%;
   
    
   img{
    width: 60%;
   }
    
 }
</style>