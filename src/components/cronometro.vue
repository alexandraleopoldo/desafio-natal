<script setup>
import presentes from "../assets/presentes.png"
</script>

<template>
  <section>
    <h2>Tempo limitado</h2>
    <p>Nessas festas de fim de ano mande um presente para a pessoa amada e compartilhe a alegria do Natal.</p>
    <h2 class="tempo">10d -24h - 01m  - 52s</h2>
    <img :src="presentes" alt="">

  </section>
</template>

<style scoped lang="scss">
    section {
        display: flex;
        flex-direction: column;
    }

    .tempo {
      font-size: 26px;
    }

</style>