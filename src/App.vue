<template>
  <div class="topo border-gray-200  flex justify-center  pt-3">
    <div class="container ">
      <HeaderPage @sobre="lenis.scrollTo('.sobrenos')" @inscrever="lenis.scrollTo('#dia-1')" @apoio="lenis.scrollTo('#apoio')" ></HeaderPage>
    </div>
  </div>
 


    <div id="tudo">
      <div class="pages overflow-x-hidden overflow-y-hidden h-screen panel flex items-center justify-center">

        <div class="relative items-center justify-center w-full overflow-x-hidden lg:pt-40 lg:pb-40 xl:pt-40 xl:pb-64">
          <div
            class="container flex flex-col items-center justify-between h-full max-w-6xl px-8 mx-auto -mt-32 lg:flex-row xl:px-0">
            <div
              class="z-30 flex flex-col items-center w-full max-w-xl pt-48 md:pt-80 text-center lg:items-start lg:w-1/2 lg:pt-20 xl:pt-40 lg:text-left">
              <h1 class="relative mb-4 text-6xl font-black leading-tight text-gray-900 sm:text-6xl xl:mb-8">Conecte-se
                com a Inovação no Cotesi</h1>
              <p class="pr-0 mb-8 text-base text-gray-600 sm:text-lg xl:text-xl lg:pr-20">Você está preparado para mais
                uma semana de tecnologia cheia de novidades?</p>
              <button
                class="relative self-start inline-block w-auto px-8 py-4 mx-auto mt-0 text-base font-bold text-white bg-blue-600 border-t border-gray-200 rounded-md shadow-xl sm:mt-1 fold-bold lg:mx-0"
                @click="lenis.scrollTo('#dia-1')">Inscreva-se
                agora</button>
              <!-- Integrates with section -->
              <div class="flex-col hidden mt-12 sm:flex lg:mt-24">
                <p class="mb-4 text-sm font-medium tracking-widest text-gray-500 uppercase">Siga-nos nas Redes Sociais
                </p>
                <div class="flex justify-center lg:justify-start transition">
                  <a href="https://www.instagram.com/ifsp.cotesi/" target="_blank">
                    <svg xmlns="http://www.w3.org/2000/svg"
                      class="h-8 mr-4 text-gray-500 duration-150 cursor-pointer fill-current transition-color hover:text-gray-600"
                      viewBox="0 0 48 48">
                      <path
                        d="M 16.5 5 C 10.16639 5 5 10.16639 5 16.5 L 5 31.5 C 5 37.832757 10.166209 43 16.5 43 L 31.5 43 C 37.832938 43 43 37.832938 43 31.5 L 43 16.5 C 43 10.166209 37.832757 5 31.5 5 L 16.5 5 z M 16.5 8 L 31.5 8 C 36.211243 8 40 11.787791 40 16.5 L 40 31.5 C 40 36.211062 36.211062 40 31.5 40 L 16.5 40 C 11.787791 40 8 36.211243 8 31.5 L 8 16.5 C 8 11.78761 11.78761 8 16.5 8 z M 34 12 C 32.895 12 32 12.895 32 14 C 32 15.105 32.895 16 34 16 C 35.105 16 36 15.105 36 14 C 36 12.895 35.105 12 34 12 z M 24 14 C 18.495178 14 14 18.495178 14 24 C 14 29.504822 18.495178 34 24 34 C 29.504822 34 34 29.504822 34 24 C 34 18.495178 29.504822 14 24 14 z M 24 17 C 27.883178 17 31 20.116822 31 24 C 31 27.883178 27.883178 31 24 31 C 20.116822 31 17 27.883178 17 24 C 17 20.116822 20.116822 17 24 17 z">
                      </path>
                    </svg>
                  </a>
                  <a href="https://www.facebook.com/ifspvotuporanga/" target="_blank">
                    <svg xmlns="http://www.w3.org/2000/svg"
                      class="h-8 mr-4 text-gray-500 duration-150 cursor-pointer fill-current transition-color hover:text-gray-600"
                      viewBox="0 0 50 50">
                      <path
                        d="M25,3C12.85,3,3,12.85,3,25c0,11.03,8.125,20.137,18.712,21.728V30.831h-5.443v-5.783h5.443v-3.848 c0-6.371,3.104-9.168,8.399-9.168c2.536,0,3.877,0.188,4.512,0.274v5.048h-3.612c-2.248,0-3.033,2.131-3.033,4.533v3.161h6.588 l-0.894,5.783h-5.694v15.944C38.716,45.318,47,36.137,47,25C47,12.85,37.15,3,25,3z">
                      </path>
                    </svg>
                  </a>
                  <a href="https://www.youtube.com/user/ifspvotuporanga" target="_blank">
                  <svg xmlns="http://www.w3.org/2000/svg"
                    class="h-8 mr-4 text-gray-500 duration-150 cursor-pointer fill-current transition-color hover:text-gray-600"
                    viewBox="0 0 50 50">
                    <path
                      d="M 44.898438 14.5 C 44.5 12.300781 42.601563 10.699219 40.398438 10.199219 C 37.101563 9.5 31 9 24.398438 9 C 17.800781 9 11.601563 9.5 8.300781 10.199219 C 6.101563 10.699219 4.199219 12.199219 3.800781 14.5 C 3.398438 17 3 20.5 3 25 C 3 29.5 3.398438 33 3.898438 35.5 C 4.300781 37.699219 6.199219 39.300781 8.398438 39.800781 C 11.898438 40.5 17.898438 41 24.5 41 C 31.101563 41 37.101563 40.5 40.601563 39.800781 C 42.800781 39.300781 44.699219 37.800781 45.101563 35.5 C 45.5 33 46 29.398438 46.101563 25 C 45.898438 20.5 45.398438 17 44.898438 14.5 Z M 19 32 L 19 18 L 31.199219 25 Z">
                    </path>
                  </svg>
                </a>
                </div>
              </div>
              <svg class="absolute left-0 max-w-md w-150 2xl:mt-24 mt-15 transition-all   -ml-120 -mt-50 2xl:-ml-64 left-svg" viewBox="0 0 423 423"
                xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                <defs>
                  <linearGradient x1="100%" y1="0%" x2="4.48%" y2="0%" id="linearGradient-1">
                    <stop stop-color="#002be5" offset="0%" />
                    <stop stop-color="#6A82E7" offset="100%" />
                  </linearGradient>
                  <filter x="-9.3%" y="-6.7%" width="118.7%" height="118.7%" filterUnits="objectBoundingBox"
                    id="filter-3">
                    <feOffset dy="8" in="SourceAlpha" result="shadowOffsetOuter1" />
                    <feGaussianBlur stdDeviation="8" in="shadowOffsetOuter1" result="shadowBlurOuter1" />
                    <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.1 0" in="shadowBlurOuter1" />
                  </filter>
                  <rect id="path-2" x="63" y="504" width="300" height="300" rx="40" />
                </defs>
                <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd" opacity=".9">
                  <g id="Desktop-HD" transform="translate(-39 -531)">
                    <g id="Hero" transform="translate(43 83)">
                      <g id="Rectangle-6" transform="rotate(45 213 654)">
                        <use fill="#000" filter="url(#filter-3)" xlink:href="#path-2" />
                        <use fill="url(#linearGradient-1)" xlink:href="#path-2" />
                      </g>
                    </g>
                  </g>
                </g>
              </svg>
            </div>
            <div class="relative z-50 flex flex-col items-end justify-center w-full h-full lg:w-1/2 ms:pl-10">
              <div class="container relative left-0  max-w-4xl lg:absolute xl:max-w-6xl md:w-screen" >
                <img src="./img/macbook-cotesi.png" fetchpriority="high" style="width: 100vw" alt="macbook-cotesi"
                  class="  mt-20 mb-20 ml-0 lg:mt-24 xl:mt-40 lg:mb-0 lg:h-full lg:-ml-12"> 
              </div>
            </div>
          </div>
        </div>


      </div>


      <SobreNos id="sobre"></SobreNos>
      <div id="pcalendar" class="pages h-auto min-h-screen p-15 panel flex items-center justify-center">

        <CalendarDate id="calendar"></CalendarDate>





      </div>
      <div class="p-1 md:p-14">
        <PatrocinadoresVue id="apoio"></PatrocinadoresVue>
      </div>

    </div>
 <FooterPage @inicio="lenis.scrollTo(0)"></FooterPage>
  
</template>

<script setup>
import HeaderPage from './components/HeaderPage.vue';
import { gsap } from "gsap";
import { onMounted, onUnmounted, ref } from 'vue';
import { ScrollTrigger } from "gsap/ScrollTrigger";
import Lenis from 'lenis';
import CalendarDate from "./components/CalendarDate.vue";
import SobreNos from "./components/SobreNos.vue";
import PatrocinadoresVue from "./components/PatrocinadoresVue.vue";
import FooterPage from './components/FooterPage.vue';

gsap.registerPlugin(ScrollTrigger);

const selected = "2025-05-08/2025-05-16";
const larguraTela = ref(window.innerWidth); // Usar ref para reatividade
let calendarTimeline = null; // Variável para armazenar a timeline do GSAP

function verificaTela() {
  return larguraTela.value > 768;
}

function initGsapCalendar() {
  if (verificaTela() && !calendarTimeline) {
    calendarTimeline = gsap.timeline({
      scrollTrigger: {
        trigger: "#pcalendar",
        toggleActions: "resume pause reverse pause",
        start: "top center",
        end: "top center",
        scrub: 3,
      },
    });

    calendarTimeline.from('#pcalendar', {
      x: 600,
      rotation: 50,
    });
  } else if (!verificaTela() && calendarTimeline) {
    // Mata a timeline se a tela for menor que 768px
    calendarTimeline.kill();
    calendarTimeline = null;
    // Reseta os estilos do elemento, se necessário
    gsap.to('#pcalendar', { clearProps: "x, rotation" });
  }
}
const lenis = new Lenis({
  autoRaf: true,
  duration: 1.2,
  autoResize: true,
});

lenis.scrollTo(0);

window.addEventListener('beforeunload', () => {
  lenis.scrollTo(0, {
    offset: 0,
    immediate: true // Tenta ir para o topo antes de descarregar
  });
})

onMounted(() => {
  // Inicializa Lenis

  // Sincroniza Lenis scrolling com GSAP's ScrollTrigger plugin
  lenis.on('scroll', ScrollTrigger.update);

  // Atualiza a largura da tela no mount
  larguraTela.value = window.innerWidth;

  // Inicializa o GSAP Calendar
  initGsapCalendar();

  // Adiciona listener para redimensionamento da tela
  window.addEventListener('resize', () => {
    larguraTela.value = window.innerWidth;
    initGsapCalendar();
  });
});

onUnmounted(() => {
  // Remove o listener de redimensionamento ao desmontar o componente
  window.removeEventListener('resize', () => { });
  // Mata a timeline se o componente for desmontado
  if (calendarTimeline) {
    calendarTimeline.kill();
    calendarTimeline = null;
  }
});
</script>
<style>
body {
  overflow-x: hidden;
  background-color: #e2e4e6;
}

button {
  cursor: pointer;
}

.cont {
  display: flex;
}

.bg-base-100 {
  background-color: #151515;
}





@media (max-width: 767px) {

  /*celular */
  .description {
    margin-top: -40%;
    padding-top: 20%;
    color: #002b5e;
    font-weight: 400;
    letter-spacing: -.03em;
    line-height: 125%;
    font-size: 4.2666666667vw;

  }
}

@media (min-width: 768px) {

  .description {
    width: 50vw;
    padding-top: 48vh;
    color: #002b5e;
    /* Ajuste para que seja maior que a altura do texto fixo */
  }

}


.test {
  border-left: 4px solid #0176ff;
  padding-left: 5px;
  width: 50%;

  line-height: 120%;
}


.tk {
  background-color: white;
}


.p {
  width: 80%;
  margin-top: 50px;
}

.p:first-child {
  margin-top: 0;
}
</style>
