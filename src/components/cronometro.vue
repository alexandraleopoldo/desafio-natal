<script setup>
import presentes from "../assets/presentes.png"
</script>

<template>
  <section>

    <div>
      <h2>Tempo limitado</h2>
      <p>Nessas festas de fim de ano mande um presente para a pessoa amada e compartilhe a alegria do Natal.</p>
      <h3>10d -24h - 01m  - 52s</h3>
      <img :src="presentes" alt="Imagem de vaŕios brinquedos juntos, formando uma pilha.">
    </div>

  </section>
</template>

<style scoped lang="scss">
    section {
        display: flex;
        flex-direction: column;
        align-items: center;
      }

    div {
        display: flex;
        flex-direction: column;
        gap: 30px;
        padding: 20px;
        margin-top: 70px;
        align-items: center;
        width: 40%;

        p {
          width: 70%;
          line-height: 30px;
          text-align: center;
          font-size: 18px;
          font-weight: 400;
        }

        h2 {
          font-weight: 600;
          font-size: 34px;
        }
        
    }

    h3 {
      font-size: 40px;
      color:  #CD3C32;
      
    }


    img {
      width: 50%;
    }
</style>