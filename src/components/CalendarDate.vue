<template>
  <div class="flex flex-wrap items-center justify-center">
    <div>
      <div class="bg-gray-800 text-white p-4 rounded-lg shadow-lg w-80">
        <div class="text-center mb-4 font-bold">MAIO</div>
        <hr class="text-gray-900">
        <div class="grid grid-cols-7">
          <div class="p-2 font-medium text-center text-sm">D</div>
          <div class="text-center p-2 font-medium text-sm">S</div>
          <div class="text-center p-2 font-medium text-sm">T</div>
          <div class="text-center p-2 font-medium text-sm">Q</div>
          <div class="text-center p-2 font-medium text-sm">Q</div>
          <div class="text-center p-2 font-medium text-sm">S</div>
          <div class="text-center p-2 font-medium text-sm">S</div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <button id="day-1" class="p-2 rounded">1</button>
          <button id="day-2" class="p-2 rounded">2</button>
          <button id="day-3" class="p-2 rounded">3</button>
          <button id="day-4" class="p-2 rounded">4</button>
          <button id="day-5" class="p-2 rounded">5</button>
          <button id="day-6" class="p-2 rounded">6</button>
          <button id="day-7" class="p-2 rounded">7</button>
          <button id="day-8" class="p-2">8</button>
          <button id="day-9" class="p-2">9</button>
          <button id="day-10" class="p-2">10</button>
          <button id="day-11" class="p-2">11</button>
          <button id="day-12" @click="selectDay(12)" class="p-2 bg-blue-600 first-date"
            :class="{ selected: selectedDay === 12 && hasBlueBg(12) }">12</button>
          <button id="day-13" @click="selectDay(13)" class="p-2 bg-blue-600"
            :class="{ selected: selectedDay === 13 && hasBlueBg(13) }">13</button>
          <button id="day-14" @click="selectDay(14)" class="p-2 bg-blue-600"
            :class="{ selected: selectedDay === 14 && hasBlueBg(14) }">14</button>
          <button id="day-15" @click="selectDay(15)" class="p-2 bg-blue-600"
            :class="{ selected: selectedDay === 15 && hasBlueBg(15) }">15</button>
          <button id="day-16" @click="selectDay(16)" class="p-2 bg-blue-600 last-date"
            :class="{ selected: selectedDay === 16 && hasBlueBg(16) }">16</button>
          <button id="day-17" class="p-2">17</button>
          <button id="day-18" class="p-2">18</button>
          <button id="day-19" class="p-2">19</button>
          <button id="day-20" class="p-2">20</button>
          <button id="day-21" class="p-2">21</button>
          <button id="day-22" class="p-2">22</button>
          <button id="day-23" class="p-2">23</button>
          <button id="day-24" class="p-2">24</button>
          <button id="day-25" class="p-2">25</button>
          <button id="day-26" class="p-2">26</button>
          <button id="day-27" class="p-2">27</button>
          <button id="day-28" class="p-2">28</button>
          <button id="day-29" class="p-2">29</button>
          <button id="day-30" class="p-2">30</button>
          <button id="day-31" class="p-2">31</button>
        </div>
      </div>
    </div>
    <div class="accordions p-5">

      <!--item 1 //  DIA 12 -->
      <div class="border-b border-slate-200">
        <button @click="toggleAccordion(12)" class="w-full flex justify-between items-center py-5 text-slate-800">
          <span id="dia-1">Dia 1: Abertura / 12 de Maio</span>
          <span id="icon-12" class="text-slate-800 transition-transform duration-300">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor" class="w-4 h-4">
              <path fill-rule="evenodd"
                d="M4.22 6.22a.75.75 0 0 1 1.06 0L8 8.94l2.72-2.72a.75.75 0 1 1 1.06 1.06l-3.25 3.25a.75.75 0 0 1-1.06 0L4.22 7.28a.75.75 0 0 1 0-1.06Z"
                clip-rule="evenodd" />
            </svg>
          </span>
        </button>
        <div id="content-12" class="max-h-0 overflow-hidden transition-all duration-300 ease-in-out">


          <div href="#"
            class="flex relative sm:flex-wrap lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #0176ff; ">
            <div class="absolute font-bold horario  bg-white z-100 rounded-e p-2">
              08:00 - 9:30h
            </div>

                <img class=" rounded-t-lg h-80 md:h-70 palestrantes  md:rounded-none md:rounded-s-lg"
              src="../img/palestrantes/LucasAlbuquerque.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">


              <div class="bg-white md:w-2/3 rounded-full text-l font-bold text-center text-white mb-1"
                style="background-color: #002b5e;">Lucas de Albuquerque</div>

              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight  text-white">Cibersegurança:
                <br> Do básico ao amanhã
              </h5>

              <p class="mb-3 font-normal text-gray-900 ">Um bate-papo descontraído sobre cibersegurança, práticas de
                proteção, privacidade, segurança em redes e
                os futuros desafios da inteligência artificial.</p>
              <a href="https://suap.ifsp.edu.br/eventos/inscricao_publica/12856/" target="_blank">
                <button
                  class="bg-white hover:bg-blue-500 w-full hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button>
              </a>
            </div>

          </div>
          <div href="#"
            class="flex sm:flex-wrap relative lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #002b5e; ">
            <div class="absolute font-bold horario  bg-white z-100 rounded-e p-2">
              10:00 - 11:30h
            </div>
                <img class=" rounded-t-lg   md:h-70 palestrantes md:rounded-none md:rounded-s-lg"
              src="../img/palestrantes/LuizBalduinoLucasAlbuquerque.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">

              <div class="bg-ac rounded text-start ps-3 mb-3 font-bold leading-5 md:w-5/6"> Lucas de Albuquerque & Luiz
                Paulo Balduíno</div>

              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight leading-6.5 text-white">Qual a Missão de Um
                Provedor
                Hoje
              </h5>

              <p class="mb-3 font-normal text-gray-900 text-white">
                Venha entender o papel crucial dos provedores de internet no
                Brasil! Exploraremos a conexão do cliente, a infraestrutura dos ISPs, desafios, segurança, inovações
                como Wi-Fi 7 e o futuro da conectividade. Uma Visão por trás dos cabos!
              </p>
              <a href="https://suap.ifsp.edu.br/eventos/inscricao_publica/12857/" target="_blank">
                <button
                  class="bg-white hover:bg-blue-500 w-full  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button>
              </a>
            </div>

          </div>
        </div>


      </div>

      <!--item 2 //  DIA 13 -->
      <div class="border-b border-slate-200">
        <button @click="toggleAccordion(13)" class="w-full flex justify-between items-center py-5 text-slate-800">
          <span>Dia 2 / 13 de Maio

          </span>

          <span id="icon-13" class="text-slate-800 transition-transform duration-300">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor" class="w-4 h-4">
              <path fill-rule="evenodd"
                d="M4.22 6.22a.75.75 0 0 1 1.06 0L8 8.94l2.72-2.72a.75.75 0 1 1 1.06 1.06l-3.25 3.25a.75.75 0 0 1-1.06 0L4.22 7.28a.75.75 0 0 1 0-1.06Z"
                clip-rule="evenodd" />
            </svg>
          </span>
        </button>
        <div id="content-13" class="max-h-0 overflow-hidden transition-all duration-300 ease-in-out">
          <div href="#"
            class="flex relative sm:flex-wrap lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #0176ff; ">
            <div class="absolute font-bold horario  bg-white z-100 rounded-e p-2">
              08:00 - 9:30h
            </div>

                <img class=" rounded-t-lg  md:h-60 palestrantes md:rounded-none md:rounded-s-lg"
              src="../img/palestrantes/RobertaSebrae.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">

              <div class="bg-white sm:w-1/2 rounded-full text-l font-bold text-center text-white mb-1"
                style="background-color: #002b5e;">Roberta Zuculoto</div>

              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight leading-6.5 leading-6.5 text-white">Mercado
                em Mutação: As Novas
                Regras do Jogo para Profissionais Inovadores</h5>

              <p class="mb-3 font-normal text-gray-900 text-gray-900">Novos modelos de negócios; Inovação; Profissão e
                Soft Skills.</p>
              <a href="https://suap.ifsp.edu.br/eventos/inscricao_publica/12791/" target="_blank">
                <button
                  class="bg-white w-full hover:bg-blue-500  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button>
              </a>
            </div>

          </div>



          <div href="#"
            class="flex sm:flex-wrap relative lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #002b5e; ">
            <div class="absolute font-bold horario  bg-white z-100 rounded-e p-2">
              10:00 - 11:30h
            </div>
                <img class=" rounded-t-lg  md:h-60 palestrantes md:rounded-none md:rounded-s-lg"
              src="../img/palestrantes/Michel.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">

              <div class="bg-ac rounded-full text-center font-bold sm:w-1/2 mb-1">Michel Rosa Simões</div>


              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight leading-6.5 text-white"> Conhecimento para
                conectar
                o mundo</h5>

              <p class="mb-3 font-normal text-gray-900 text-white">Uma visão do fascinante universo das comunicações
                ópticas e as soluções inovadoras da Furukawa, incluindo como se capacitar e se certificar para atender
                as demandas em redes de computação por Fibras Opticas, empregando melhores práticas de instalação e
                soluções capazes de revolucionar a forma como nos conectamos.</p>
              <button
                class="bg-white w-full hover:bg-blue-500  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                Inscrições Em Breve
              </button>
            </div>
          </div>

          <div href="#"
            class="flex sm:flex-wrap relative lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #0176ff; ">
            <div class="absolute font-bold horario  bg-white z-100 rounded-e p-2">
              13:00 - 16:00h
            </div>
                <img class=" rounded-t-lg  md:h-60 palestrantes md:rounded-none md:rounded-s-lg"
              src="../img/palestrantes/VitorFabio.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">
              <div class="bg-white sm:w-1/2 rounded-full text-l font-bold text-center text-white mb-1"
                style="background-color: #002b5e;">Vitor Fábio</div>
              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight leading-6.5 text-white">Oficina -
                Desbravando o
                Laravel: Construindo Aplicações Web Modernas com PHP</h5>

              <p class="mb-3 font-normal text-gray-900">Oficina introdutória ao Laravel (framework PHP):
                explore conceitos, arquitetura MVC, rotas, controllers, Blade, Eloquent ORM, autenticação e comandos
                Artisan. Ideal para entender aplicações Laravel e desenvolver projetos com produtividade.</p>
              <a href="https://suap.ifsp.edu.br/eventos/inscricao_publica/12802/" target="_blank">
                <button
                  class="bg-white w-full hover:bg-blue-500  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button></a>
            </div>
          </div>

          <div href="#"
            class="flex relative sm:flex-wrap lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #002b5e; ">
            <div class="absolute font-bold horariotr bg-white z-100 rounded-e p-2">
              8:00 - 17:00h
            </div>

                <img class=" rounded-t-lg  md:h-60  md:rounded-none md:rounded-s-lg" src="../img/cabeamentos.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">

              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight  text-white">Treinamento Lightera(Furukawa)
                - FCP Fibras
                Opticas (parte 1 de 4): Introdução às Fibras Ópticas</h5>

              <p class="mb-3 font-normal text-white">Treinamento profissional <span class="font-bold">Gratuito</span>,
                saiba mais no link (Confira os termos).</p>
              <a href="https://forms.gle/RHxGTxDP94BXxy8FA" target="_blank">
                <button
                  class="bg-white hover:bg-blue-500 w-full  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button>
              </a>
            </div>
          </div>

        </div>
      </div>

      <!--item 3 //  DIA 14 -->
      <div class="border-b border-slate-200 ">
        <button @click="toggleAccordion(14)" class="w-full flex justify-between items-center py-5 text-slate-800">
          <span>Dia 3 / 14 de Maio</span>
          <span id="icon-14" class="text-slate-800 transition-transform duration-300">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor" class="w-4 h-4">
              <path fill-rule="evenodd"
                d="M4.22 6.22a.75.75 0 0 1 1.06 0L8 8.94l2.72-2.72a.75.75 0 1 1 1.06 1.06l-3.25 3.25a.75.75 0 0 1-1.06 0L4.22 7.28a.75.75 0 0 1 0-1.06Z"
                clip-rule="evenodd" />
            </svg>

          </span>
        </button>
        <div id="content-14" class="max-h-0 overflow-hidden transition-all duration-300 ease-in-out">
          <div href="#"
            class="flex relative sm:flex-wrap lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #0176ff; ">
            <div class="absolute font-bold horario  bg-white z-100 rounded-e p-2">
              08:00 - 9:30h
            </div>

                <img class=" rounded-t-lg h-70  palestrantesq md:rounded-none md:rounded-s-lg"
              src="../img/palestrantes/AntonioProdesp.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">

              <div class="bg-white sm:w-1/2 rounded-full text-l font-bold text-center text-white mb-1"
                style="background-color: #002b5e;">Antônio (Prodesp)</div>
              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight leading-6.5 text-white">Do Analista de
                Requisitos ao
                Product Owner: Navegando pelos Papéis em Negócios e Tecnologia</h5>

              <p class="mb-3 font-normal text-gray-900 text-gray-900">Analista de Requisitos, Negócios e Product Owner:
                diferenças, sinergias, mercado e tendências para profissionais multifuncionais na área.</p>

              <a href="https://suap.ifsp.edu.br/eventos/inscricao_publica/12792/" target="_blank">
                <button
                  class="bg-white w-full hover:bg-blue-500  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button>
              </a>
            </div>
          </div>


          <div href="#"
            class="flex sm:flex-wrap relative lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #002b5e; ">
            <div class="absolute font-bold horario  bg-white z-100 rounded-e p-2">
              10:00 - 11:30h
            </div>
                <img class=" rounded-t-lg  md:h-60 palestrantes md:rounded-none md:rounded-s-lg"
              src="../img/palestrantes/MarianaDuarte.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">
              <div class="bg-ac rounded-full text-center font-bold sm:w-1/2 mb-1">Mariana Duarte</div>
              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight leading-6.5 text-white">Tecnologia em
                Movimento: Como
                os Dados Estão Transformando a Mobilidade Urbana</h5>

              <p class="mb-3 font-normal text-gray-900 text-white">Venha entender como Dados de mobilidade urbana
                monitorados otimizam transporte e planejamento</p>
              <a href="https://suap.ifsp.edu.br/eventos/inscricao_publica/12793/" target="_blank">
                <button
                  class="bg-white w-full hover:bg-blue-500  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button>
              </a>
            </div>
          </div>


          <div href="#"
            class="flex relative sm:flex-wrap lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #0176ff; ">
            <div class="absolute font-bold horario  bg-white z-100 rounded-e p-2">
              13:00 - 16:00h
            </div>

                <img class=" rounded-t-lg h-70  palestrantesq md:rounded-none md:rounded-s-lg"
              src="../img/palestrantes/Josue.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">

              <div class="bg-ae sm:w-1/2 rounded-full text-l font-bold text-center text-white mb-1">Josué Teodoro</div>

              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight leading-6.5 text-white">Oficina - Criando
                Sites com
                Python: Introdução ao Django</h5>

              <p class="mb-3 font-normal text-gray-900 text-gray-900">
                Python e Django para iniciantes: crie seu primeiro
                site e entenda o desenvolvimento web.
              </p>
              <a href="https://suap.ifsp.edu.br/eventos/inscricao_publica/12801/" target="_blank">
                <button
                  class="bg-white w-full hover:bg-blue-500  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button>
              </a>
            </div>
          </div>

          <div href="#"
            class="flex relative sm:flex-wrap lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #002b5e; ">
            <div class="absolute font-bold horariotr bg-white z-100 rounded-e p-2">
              9:00 - 16:00h
            </div>

                <img class=" rounded-t-lg  md:h-60  md:rounded-none md:rounded-s-lg" src="../img/cabeamentos.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">

              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight  text-white">Treinamento Lightera(Furukawa)
                - FCP Fibras
                Opticas (parte 2 de 4): Instalação de Redes Ópticas</h5>

              <p class="mb-3 font-normal text-white">Treinamento profissional <span class="font-bold">Gratuito</span>,
                saiba mais no link (Confira os termos).</p>
              <a href="https://forms.gle/RHxGTxDP94BXxy8FA" target="_blank">
                <button
                  class="bg-white hover:bg-blue-500 w-full  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button>
              </a>
            </div>
          </div>

        </div>
      </div>

      <!--item 4 //  DIA 15 -->
      <div class="border-b border-slate-200 ">
        <button @click="toggleAccordion(15)" class="w-full flex justify-between items-center py-5 text-slate-800">
          <span>Dia 4 / 15 de Maio</span>
          <span id="icon-15" class="text-slate-800 transition-transform duration-300">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor" class="w-4 h-4">
              <path fill-rule="evenodd"
                d="M4.22 6.22a.75.75 0 0 1 1.06 0L8 8.94l2.72-2.72a.75.75 0 1 1 1.06 1.06l-3.25 3.25a.75.75 0 0 1-1.06 0L4.22 7.28a.75.75 0 0 1 0-1.06Z"
                clip-rule="evenodd" />
            </svg>

          </span>
        </button>
        <div id="content-15" class="max-h-0 overflow-hidden transition-all duration-300 ease-in-out">
          <div href="#"
            class="flex relative sm:flex-wrap lg:flex-nowrap flex-col items-center bg-white border mt-15 mb-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #0176ff; ">
            <div class="absolute font-bold horario  bg-white z-100 rounded-e p-2">
              08:00 - 9:30h
            </div>

                <img class=" rounded-t-lg  md:h-60 palestrantes md:rounded-none md:rounded-s-lg"
              src="../img/palestrantes/AlessandroLopes.png">

                <div class="flex relative  mt-7 flex-col cards justify-between p-4 leading-normal">
              <div class="bg-ae sm:w-1/2 rounded-full text-l font-bold text-center text-white mb-1 mb-2">Alessandro Lopes</div>
              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight leading-6.5 text-white">IA GENERATIVA COM
                .NET</h5>

              <p class="mb-3 font-normal text-gray-900 text-gray-900">Venha conosco aprender como criar aplicativos mais
                inteligentes de forma rápida com IA Generativa em .NET</p>
              <a href="https://suap.ifsp.edu.br/eventos/inscricao_publica/12795/" target="_blank"><button
                  class="bg-white hover:bg-blue-500 w-full hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button></a>
            </div>
          </div>


          <div href="#"
            class="flex sm:flex-wrap relative lg:flex-nowrap flex-col items-center mt- bg-white border  border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #002b5e; ">
            <div class="absolute font-bold horario  bg-white z-100 rounded-e p-2">
              10:00 - 11:30h
            </div>
                <img class=" rounded-t-lg  md:h-60 palestrantes md:rounded-none md:rounded-s-lg"
              src="../img/palestrantes/JoaoCarlos.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">

              <div class="bg-ac rounded-full text-center font-bold sm:w-1/2 mb-1">João Carlos</div>

              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight leading-6.5 text-white">GitHub além do
                código -
                desenvolvendo pessoas, não só software</h5>

              <p class="mb-3 font-normal text-gray-900 text-white">João Carlos mostra que GitHub é mais que código, é um
                espaço para aprender, colaborar e crescer na tecnologia.</p>
              <a href="https://suap.ifsp.edu.br/eventos/inscricao_publica/12796/" target="_blank">
                <button
                  class="bg-white w-full hover:bg-blue-500  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button>
              </a>
            </div>

          </div>

          <div href="#"
            class="flex relative sm:flex-wrap lg:flex-nowrap flex-col items-center bg-white border mt-15 mb-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #0176ff; ">
            <div class="absolute font-bold horario  bg-white z-100 rounded-e p-2">
              13:00 - 16:00h
            </div>

                <img class=" rounded-t-lg  h-70 palestrantesq md:rounded-none md:rounded-s-lg"
              src="../img/palestrantes/EvelynAmaral.png">

                <div class="flex relative  mt-7 flex-col cards justify-between p-4 leading-normal">

              <div class="bg-ae sm:w-1/2 rounded-full text-l font-bold text-center text-white mb-1"
               >Evelyn Amaral</div>

              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight leading-6.5 text-white">Princípios Básicos e
                Configuração de Redes LAN</h5>

              <p class="mb-3 font-normal text-gray-900 text-gray-900">Aprenda os fundamentos das redes locais (LAN),
                conheça os principais protocolos utilizados em redes domésticas e descubra como configurar sua própria
                rede de forma prática e eficiente.</p>
              <a href="https://suap.ifsp.edu.br/eventos/inscricao_publica/12850/" target="_blank"><button
                  class="bg-white hover:bg-blue-500 w-full hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button></a>
            </div>
          </div>


          <div href="#"
            class="flex relative sm:flex-wrap lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #002b5e ">
            <div class="absolute font-bold horariotr bg-white z-100 rounded-e p-2">
              9:00 - 16:00h
            </div>

                <img class=" rounded-t-lg  md:h-60  md:rounded-none md:rounded-s-lg" src="../img/cabeamentos.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">

              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight  text-white">Treinamento Lightera(Furukawa)
                - FCP Fibras
                Opticas (parte 3 de 4): Projeto e Certificação de Redes Ópticas</h5>

              <p class="mb-3 font-normal text-white">Treinamento profissional <span class="font-bold">Gratuito</span>,
                saiba mais no link (Confira os termos).</p>
              <a href="https://forms.gle/RHxGTxDP94BXxy8FA" target="_blank">
                <button
                  class="bg-white hover:bg-blue-500 w-full  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button>
              </a>
            </div>
          </div>

        </div>
      </div>

      <!--item 5 //  DIA 16 -->
      <div class="border-b border-slate-200 ">

        <button @click="toggleAccordion(16)" class="w-full flex justify-between items-center py-5 text-slate-800">
          <span>Dia 5: Fechamento / 16 de Maio</span>
          <span id="icon-16" class="text-slate-800 transition-transform duration-300">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor" class="w-4 h-4">
              <path fill-rule="evenodd"
                d="M4.22 6.22a.75.75 0 0 1 1.06 0L8 8.94l2.72-2.72a.75.75 0 1 1 1.06 1.06l-3.25 3.25a.75.75 0 0 1-1.06 0L4.22 7.28a.75.75 0 0 1 0-1.06Z"
                clip-rule="evenodd" />
            </svg>

          </span>
        </button>
        <div id="content-16" class="max-h-0 overflow-hidden transition-all duration-300 ease-in-out">
          <div href="#"
            class="flex relative sm:flex-wrap lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #0176ff; ">
            <div class="absolute font-bold horario  bg-white z-100 rounded-e p-2">
              08:00 - 9:30h
            </div>

                <img class=" rounded-t-lg  md:h-60 palestrantes md:rounded-none md:rounded-s-lg"
              src="../img/palestrantes/LucasRibeiro.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">

              <div class="bg-ae sm:w-1/2 rounded-full text-l font-bold text-center text-white mb-1"
               >Lucas Ribeiro</div>

              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight leading-6.5 text-white">Além do Código: Como
                a
                Flexibilidade Impulsiona sua Carreira</h5>

              <p class="mb-3 font-normal text-gray-900 text-gray-900">Veja como experiências práticas e mudanças no
                mercado ensinam que adaptar-se é a chave para crescer na carreira tech.</p>

              <a href="https://suap.ifsp.edu.br/eventos/inscricao_publica/12798/" target="_blank">
                <button
                  class="bg-white w-full hover:bg-blue-500  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button>
              </a>
            </div>

          </div>
          <div href="#"
            class="flex sm:flex-wrap relative lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #002b5e; ">
            <div class="absolute font-bold horario  bg-white z-100 rounded-e p-2">
              10:00 - 11:30h
            </div>
                <img class=" rounded-t-lg  md:h-60 palestrantes  md:rounded-none md:rounded-s-lg"
              src="../img/palestrantes/Cami.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">

              <div class="bg-ac rounded-full text-center font-bold md:sm:w-1/2 mb-1">Cami Martins</div>

              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight leading-6.5 text-white">Performance de Rede
                com
                Cilium, eBPF e Gemini</h5>

              <p class="mb-3 font-normal text-gray-900 text-white">Acompanhe como Cilium, eBPF e Gemini otimizam redes
                Kubernetes/Cloud-Native para performance, segurança e escalabilidade de microsserviços.</p>
              <a href="https://suap.ifsp.edu.br/eventos/inscricao_publica/12799/" target="_blank">
                <button
                  class="bg-white w-full hover:bg-blue-500  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button>
              </a>
            </div>

          </div>


          <div href="#"
            class="flex relative sm:flex-wrap lg:flex-nowrap flex-col items-center bg-white border mt-15 border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100  bg-gray-800 hover:bg-gray-700"
            style="background-color: #0176ff; ">
            <div class="absolute font-bold horariotr bg-white z-100 rounded-e p-2">
              9:00 - 13:00h
            </div>

                <img class=" rounded-t-lg  md:h-60  md:rounded-none md:rounded-s-lg" src="../img/cabeamentos.png">

                <div class="flex relative flex-col cards justify-between p-4 leading-normal">

              <h5 class="mb-2 text-2xl font-bold leading-6.5 tracking-tight  text-white">Treinamento Lightera(Furukawa)
                - FCP Fibras
                Opticas (parte 4 de 4): Prática e Montagem de Redes Ópticas</h5>

              <p class="mb-3 font-normal text-gray-900 text-gray-900">Treinamento profissional <span
                  class="font-bold">Gratuito</span>, saiba mais no link (Confira os termos).</p>
              <a href="https://forms.gle/RHxGTxDP94BXxy8FA" target="_blank">
                <button
                  class="bg-white hover:bg-blue-500 w-full  hover:scale-105 hover:bg-gray-300 transition-all text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
                  Inscreva-se
                </button>
              </a>
            </div>
          </div>

        </div>
      </div>

    </div>
  </div>
</template>
<script setup>
import { ref, onMounted } from 'vue';

const selectedDay = ref(null);

function hasBlueBg(day) {
  const element = document.getElementById(`day-${day}`);
  return element && element.classList.contains('bg-blue-600');
}
function selectDay(day) {
  selectedDay.value = day;
  toggleAccordion(day)
  hasBlueBg(day)

}
onMounted(() => {


  const diaMes = new Date().toLocaleDateString('pt-BR', {
    day: 'numeric'
  })









})

function toggleAccordion(index) {
  const content = document.getElementById(`content-${index}`);
  const icon = document.getElementById(`icon-${index}`);

  // SVG for Down icon
  const downSVG = `
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor" class="w-4 h-4">
      <path fill-rule="evenodd" d="M4.22 6.22a.75.75 0 0 1 1.06 0L8 8.94l2.72-2.72a.75.75 0 1 1 1.06 1.06l-3.25 3.25a.75.75 0 0 1-1.06 0L4.22 7.28a.75.75 0 0 1 0-1.06Z" clip-rule="evenodd" />
    </svg>
  `;

  // SVG for Up icon
  const upSVG = `
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor" class="w-4 h-4">
      <path fill-rule="evenodd" d="M11.78 9.78a.75.75 0 0 1-1.06 0L8 7.06 5.28 9.78a.75.75 0 0 1-1.06-1.06l3.25-3.25a.75.75 0 0 1 1.06 0l3.25 3.25a.75.75 0 0 1 0 1.06Z" clip-rule="evenodd" />
    </svg>
  `;

  // Fechar todos os outros accordions
  for (let i = 12; i <= 16; i++) { // Ajuste os limites conforme necessário
    if (i !== index) {
      const otherContent = document.getElementById(`content-${i}`);
      const otherIcon = document.getElementById(`icon-${i}`);
      if (otherContent && otherContent.style.maxHeight && otherContent.style.maxHeight !== '0px') {
        otherContent.style.maxHeight = '0';
        if (otherIcon) {
          otherIcon.innerHTML = downSVG;
        }
      }
    }
  }

  // Abrir/fechar o accordion selecionado
  if (content.style.maxHeight && content.style.maxHeight !== '0px') {
    content.style.maxHeight = '0';
    icon.innerHTML = downSVG;
  } else {
    content.style.maxHeight = content.scrollHeight + 'px';
    icon.innerHTML = upSVG;
  }


}
</script>

<style scoped>
.first-date {
  border-top-left-radius: 0.5rem;
  border-bottom-left-radius: 0.5rem;
}

.last-date {
  border-top-right-radius: 0.5rem;
  border-bottom-right-radius: 0.5rem;
}

.grid-cols-7 {
  grid-template-columns: repeat(7, 1fr);
}

button.bg-blue-600:hover {
  cursor: pointer;
  /* Adiciona o cursor de ponteiro aos botões */
  background-color: #e2e4e6;
  color: black;
}

button.selected {
  background-color: #e2e4e6;
  color: black;
}

.horario {
  top: 175px;
  left: 0;
}

.horariotr {
  top: 200px;
  left: 0;
}

.palestrantes {
  position: relative;
  top: -60px;
}

.palestrantesq {
  position: relative;
  top: -40px;
}

.bg-ac {
  background-color: #0176ff;
  color: white;
}

.bg-ae {
  background-color: #002b5e;
  color: white;
}
</style>