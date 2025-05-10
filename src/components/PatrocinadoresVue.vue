<template>
  <div  class="h-full w-full mb-15 pt-15">

    <h2 class="text-blue-600 font-sans text-lg  mb-2 text-center">Confiam no Nosso Projeto</h2>
    <h3 class="relative text-center  font-black text-xl  mb-5 xl:mb-8 text-gray-800 sm:text-5xl ">APOIADORES</h3>
    <swiper   :slides-per-view="3" 
    :breakpoints="{768: {slidesPerView: 5} }" 
    :autoplay="{ // Configurações do autoplay
        delay: 2000, // Tempo em milissegundos entre os slides (opcional, padrão é 3000)
        disableOnInteraction: false, // Permite que o autoplay continue mesmo após a interação do usuário (opcional, padrão é true)
        pauseOnMouseEnter: true, // Pausa o autoplay ao passar o mouse (opcional, padrão é false)
        // reverseDirection: false, // Descomente para inverter a direção (opcional, padrão é false)
      }"
      :navigation="navigationEnabled ? { hideOnClick: true } : larguraTela>768"
    :centered-slides="true"
    :loop="true"
      class="h-full overflow-x-hidden w-full select-none ">
      
      
      <swiper-slide >
        <a class="h-full w-full ts-swiper" target="_blank" href="https://www.facchini.com.br/"><img loading="lazy" src="../img/patrocinadores/facchini-logo.png" alt="Logo Facchini"></a>
      </swiper-slide>
      <swiper-slide>
        <a target="_blank" href="https://www.flashnetbrasil.com.br/" class="ts-swiper"><img loading="lazy"  src="../img/patrocinadores/flash-logo.png" alt="Logo Flash Net"></a>
      </swiper-slide>
      <swiper-slide>
        <a target="_blank" href="https://itepbrasil.net/site/" class="ts-swiper"><img loading="lazy"  src="../img/patrocinadores/ITEPBrasil.png" alt="Logo Itep Brasil"></a>
      </swiper-slide>
      <swiper-slide>
        <a target="_blank" href="https://github.com/" class="ts-swiper flex items-center h-full"><img loading="lazy" width="156px" src="../img/patrocinadores/GitHub.svg" alt="Logo GitHub"></a>
      </swiper-slide>
      
      <swiper-slide>
        <a class="ts-swiper " target="_blank" href="https://www.instagram.com/leticiaamandadoceria/"><img loading="lazy" src="../img/patrocinadores/logoleticia.png" alt="Logo Leticia Amanda Doceria"></a>
      </swiper-slide
      >
      <swiper-slide>
        <a target="_blank" href="https://www.papinipremoldados.com.br/" class="ts-swiper"><img loading="lazy"  src="../img/patrocinadores/logopapini.png" alt="Logo Papini Pré-Moldados"></a>
      </swiper-slide>
      <swiper-slide>
        <a target="_blank" href="http://www.institutolabruma.com.br/" class="ts-swiper"><img loading="lazy"  src="../img/patrocinadores/labruma.svg" alt="Logo LaBruma"></a>
      </swiper-slide>
      <swiper-slide>
        <a target="_blank" href="https://www.furukawalatam.com/pt-br" class="ts-swiper"><img loading="lazy"  src="../img/patrocinadores/lightera.svg" alt="Logo Lightera"></a>
      </swiper-slide>
      
      
      

    </swiper>

    
  </div>
</template>
<script setup>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// import Swiper core and required modules
// swiper bundle styles
import "swiper/element/css/autoplay"
import "swiper/css/bundle";
import { onMounted,ref } from 'vue';

const autoplayConfig = ref(false); // Inicialmente desabilitado

const larguraTela = ref(window.innerWidth); // Usar ref para reatividade



</script>
<style scoped>
.ts-swiper {
  display: flex;
  justify-content: center;
}



.swiper-slide {
  /* Estilos base dos seus slides */
  opacity: 0.95; /* Opcional: para dar um destaque menor aos outros slides */
  transition: transform 0.3s ease-in-out, opacity 0.3s ease-in-out; /* Adiciona uma transição suave */
  
}

.swiper-slide-active {
  transform: scale(1.3); /* Aumenta o tamanho do slide ativo em 10% */
  opacity: 1; /* Garante que o slide ativo esteja totalmente visível */
  z-index: 1; /* Garante que o slide ativo não seja sobreposto pelos vizinhos */
  transform: translateY(-2px);
}
</style>