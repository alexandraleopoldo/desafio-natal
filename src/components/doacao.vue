<script setup>
import enfeite from "../assets/enfeite-mao.png"
</script>

<template>
    <section>
        <img :src="enfeite" alt="">
        <div>
            <h2>Conectando generosidade
                ao redor do mundos</h2>
            <p>Celebre a magia do Natal de uma maneira especial! Descubra a plataforma que permite a doação de presentes significativos para aqueles que mais precisam. Faça parte do movimento e compartilhe o verdadeiro espírito da generosidade.</p>
            <a href="https://doacoes.criancaesperanca.unesco.org/" target="_blank"><button>FAZER UMA DOAÇÃO</button></a>
        </div>
    </section>
</template>

<style scoped lang="scss">
    section {
        display: flex;
        justify-content: space-around;
        align-items: center;
        gap: 40px;
        img {
            width: 30%;
        }
    }
</style>