<script setup>
import enfeite from "../assets/enfeite-mao.png"

const doacao = () => {
  window.open("https://doacoes.criancaesperanca.unesco.org/", "_blank");
};
</script>

<template>
    <section>
        <img :src="enfeite" alt="">
        <div>
            <h2>Conectando generosidade
                ao redor do mundo</h2>
            <p>Celebre a magia do Natal de uma maneira especial! Descubra a plataforma que permite a doação de presentes significativos para aqueles que mais precisam. Faça parte do movimento e compartilhe o verdadeiro espírito da generosidade.</p>
            <button @click="doacao" class="estilo-button">FAZER UMA DOAÇÃO</button>
        </div>
    </section>
</template>

<style scoped lang="scss">
    section {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        background-color: #FFE9E8;
        gap: 40px;
        height: 600px;
        margin-top: 30px;
        img {
            width: 16%;
        }
    }

    div {
        display: flex;
        flex-direction: column;
        gap: 30px;
        padding: 20px;
        margin-top: 20px;
        width: 30%;
        

        p {
          width: 80%;
          line-height: 30px;
          font-size: 20px;
          font-weight: 400;
        }

        h2 {
          font-weight: 600;
          font-size: 34px;
          width: 90%;
        }
    }
</style>