<template>
  <div class="pages pagetitle lg:flex md:flex">
    <div class="title panel h-screen text-gray-900  text-7xl sm:text-8xl mb-20 flex items-center justify-center"
      style="font-family: 'TuskerGrotesk'; width: 50vw; ">
      <div id="title" class="test text-wrap">

        O QUE É COTESI?
      </div>
    </div>

    <div class="description panel  flex-wrap flex items-center justify-center " style="margin-bottom: 10vh;">
      <div class="description panel sobrenos flex-wrap flex items-center justify-center " style="margin-bottom: 10vh;">
        <div class="p ">
          O X Congresso de Tecnologia e Sistemas de Informação (COTESI) é uma iniciativa do corpo docente e dicente da área tecnológica
          do Câmpus Votuporanga. Este evento compreende a realização de palestras e minicursos direcionados
          ao
          campo da tecnologia, com o intuito de disseminar conhecimento e promover a interação entre acadêmicos e a
          comunidade.
        </div>
        <div class="p mt-10">
          A organização do COTESI está a cargo de uma comissão designada, composta por representantes do corpo docente e
          discente dos cursos de graduação em Sistemas de Informação. Este esforço conjunto visa assegurar a relevância
          e a
          qualidade do evento para todos os participantes.
        </div>
        <div class="p mt-10">
          O congresso tem como objetivo principal complementar a formação acadêmica dos estudantes, proporcionando um
          panorama das tendências e das práticas no setor de Tecnologia da Informação. As palestras e minicursos
          abordarão
          temáticas relacionadas ao Ensino, à Pesquisa e à Extensão, pilares fundamentais da educação superior.
        </div>
        <div class="p mt-10">
          Adicionalmente, o COTESI dedicará espaço à discussão de temas transversais de significativa importância
          social e ambiental, como Meio Ambiente & Sustentabilidade e Responsabilidade Social, reconhecendo a relevância
          destes aspectos para a formação integral dos participantes.
        </div>
        <div class="p mt-10 ultimo">
          Este evento é oferecido de forma gratuita e aberta à participação de toda a comunidade interessada em
          tecnologia
          e áreas correlatas. Convidamos você a aproveitar esta oportunidade para expandir seus conhecimentos,
          estabelecer
          conexões e participar de um debate enriquecedor. <span class="font-bold">Sua presença é valiosa!</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { onMounted, onUnmounted, ref } from 'vue';
import { gsap } from "gsap";
import { ScrollTrigger } from "gsap/ScrollTrigger";

gsap.registerPlugin(ScrollTrigger);

const larguraTela = ref(window.innerWidth);
let titleTimeline = null;
let pinTrigger = null;

function verificaTela() {
  return larguraTela.value > 800;
}

function initGsapTitle() {
  if (verificaTela() && !titleTimeline) {

    titleTimeline = gsap.timeline({
      scrollTrigger: {
        trigger: "#title",
        toggleActions: "resume pause reverse pause",
        start: "bottom center",
        end: "bottom 50px",
        scrub: 3,
      },
    });

    titleTimeline.from('#title', {
      x: -100,
      duration: 3,
    });

    pinTrigger = ScrollTrigger.create({
      id: "pinTrigger", // Adicione um ID para facilitar a busca
      trigger: ".title",
      endTrigger: ".description",
      start: "top top",
      end: "bottom 70%",
      pin: true,
      invalidateOnRefresh: true,
    });

  } else if (!verificaTela()) {
    if (titleTimeline) {
      titleTimeline.kill();
      titleTimeline = null;
    }
    if (pinTrigger) {
      pinTrigger.kill();
      pinTrigger = null;
    }
    gsap.to('#title', { clearProps: "x, position, top, left, bottom, right, width" }); // Limpa as props de pin
  } else if (verificaTela() && titleTimeline && !ScrollTrigger.getById("pinTrigger")) {
    pinTrigger = ScrollTrigger.create({
      id: "pinTrigger",
      trigger: ".title",
      start: "top top",
      end: "bottom 65%",
      pin: true,
      invalidateOnRefresh: true,
    });
  }
}

onMounted(() => {
  larguraTela.value = window.innerWidth;
  initGsapTitle();

  window.addEventListener('resize', () => {

    larguraTela.value = window.innerWidth;
    initGsapTitle();
  });
});

onUnmounted(() => {
  if (titleTimeline) {
    titleTimeline.kill();
    titleTimeline = null;
  }
  if (pinTrigger) {
    pinTrigger.kill();
    pinTrigger = null;
  }
  window.removeEventListener('resize', () => { });
});
</script>



<style lang="">

</style>