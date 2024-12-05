<script setup>
import presentes from "../assets/presentes.png";
import { ref, computed, onMounted, onBeforeUnmount } from "vue";

const tempoRestante = ref(1 * 2 * 60 * 60); 


let idIntervalo;
onMounted(() => {
  idIntervalo = setInterval(() => {
    if (tempoRestante.value > 0) {
      tempoRestante.value--; 
    } else {
      clearInterval(idIntervalo); 
    }
  }, 1000);
});


onBeforeUnmount(() => {
  clearInterval(idIntervalo);
});


const tempoFormatado = computed(() => {
  if (tempoRestante.value <= 0) return "Tempo Esgotado!"; 
  const dias = Math.floor(tempoRestante.value / (24 * 60 * 60));
  const horas = Math.floor((tempoRestante.value % (24 * 60 * 60)) / (60 * 60));
  const minutos = Math.floor((tempoRestante.value % (60 * 60)) / 60);
  const segundos = tempoRestante.value % 60;
  return `${dias}d - ${horas}h - ${minutos}m - ${segundos}s`;
});

</script>

<template>
  <section>
    <div>
      <h2>Tempo limitado</h2>
      <p>
        Nessas festas de fim de ano mande um presente para a pessoa amada e
        compartilhe a alegria do Natal.
      </p>
      <h3>{{ tempoFormatado }}</h3>
      <img :src="presentes" alt="Imagem de vários brinquedos juntos, formando uma pilha." />
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
}

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

h3 {
  font-size: 40px;
  color: #cd3c32;
}

img {
  width: 50%;
}
</style>
