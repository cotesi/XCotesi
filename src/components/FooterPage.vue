<template lang="">
  <footer class="w-full py-7 text-white " style="background-color: #002b5e; ">
    
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
      <div class="max-w-3xl mx-auto">
        <div class=" w-60 mx-auto rounded">
          <img loading="lazy" class="h-20 mx-auto" src="../img/logo2.svg">
          
        </div>
        <div class="flex mx-auto w-full justify-center items-center flex-col">
          <h3 class='text-center text-xl'>Realização:</h3>
          <div class="flex flex-1 mt-5">
            <img class="h-25 -mt-5" src="../img/logobsi.png">
            <div
            class="h-[25px] min-h-[1em] w-px self-stretch bg-gradient-to-tr from-transparent via-white-500 to-transparent  "></div>
            <img class="h-25 -mt-5" src="../img/ifsplogo.png">
          </div>
        </div>
        <div class="text-lg  flex flex-col items-center justify-center  gap-7  md:gap-3 transition-all duration-500 p-10 mb-10 border-b border-gray-200">
          <button @click="emitTopo()" class="hover:text-gray-600">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class=" size-10">
        <path stroke-linecap="round" stroke-linejoin="round" d="m15 11.25-3-3m0 0-3 3m3-3v7.5M21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
        </svg>
      </button>
        Voltar ao Topo
        </div>
        
        <div class="flex space-x-10 justify-center items-center mb-14">
          <a href="https://www.instagram.com/ifsp.cotesi/" target="_blank">
            <svg xmlns="http://www.w3.org/2000/svg"
            class="h-8 mr-4  duration-150 cursor-pointer fill-current transition-color hover:text-gray-600"
            viewBox="0 0 48 48">
            <path
            d="M 16.5 5 C 10.16639 5 5 10.16639 5 16.5 L 5 31.5 C 5 37.832757 10.166209 43 16.5 43 L 31.5 43 C 37.832938 43 43 37.832938 43 31.5 L 43 16.5 C 43 10.166209 37.832757 5 31.5 5 L 16.5 5 z M 16.5 8 L 31.5 8 C 36.211243 8 40 11.787791 40 16.5 L 40 31.5 C 40 36.211062 36.211062 40 31.5 40 L 16.5 40 C 11.787791 40 8 36.211243 8 31.5 L 8 16.5 C 8 11.78761 11.78761 8 16.5 8 z M 34 12 C 32.895 12 32 12.895 32 14 C 32 15.105 32.895 16 34 16 C 35.105 16 36 15.105 36 14 C 36 12.895 35.105 12 34 12 z M 24 14 C 18.495178 14 14 18.495178 14 24 C 14 29.504822 18.495178 34 24 34 C 29.504822 34 34 29.504822 34 24 C 34 18.495178 29.504822 14 24 14 z M 24 17 C 27.883178 17 31 20.116822 31 24 C 31 27.883178 27.883178 31 24 31 C 20.116822 31 17 27.883178 17 24 C 17 20.116822 20.116822 17 24 17 z">
                      </path>
                    </svg>
                  </a>
                  
                  <a href="https://www.facebook.com/ifspvotuporanga/" target="_blank">
                    <svg xmlns="http://www.w3.org/2000/svg"
                    class="h-8 mr-4  duration-150 cursor-pointer fill-current transition-color hover:text-gray-600"
                    viewBox="0 0 50 50">
                    <path
                        d="M25,3C12.85,3,3,12.85,3,25c0,11.03,8.125,20.137,18.712,21.728V30.831h-5.443v-5.783h5.443v-3.848 c0-6.371,3.104-9.168,8.399-9.168c2.536,0,3.877,0.188,4.512,0.274v5.048h-3.612c-2.248,0-3.033,2.131-3.033,4.533v3.161h6.588 l-0.894,5.783h-5.694v15.944C38.716,45.318,47,36.137,47,25C47,12.85,37.15,3,25,3z">
                      </path>
                    </svg>
                  </a>
                  <a href="https://www.youtube.com/user/ifspvotuporanga" target="_blank">
                    <svg xmlns="http://www.w3.org/2000/svg"
                    class="h-8 mr-4  duration-150 cursor-pointer fill-current transition-color hover:text-gray-600"
                    viewBox="0 0 50 50">
                    <path
                    d="M 44.898438 14.5 C 44.5 12.300781 42.601563 10.699219 40.398438 10.199219 C 37.101563 9.5 31 9 24.398438 9 C 17.800781 9 11.601563 9.5 8.300781 10.199219 C 6.101563 10.699219 4.199219 12.199219 3.800781 14.5 C 3.398438 17 3 20.5 3 25 C 3 29.5 3.398438 33 3.898438 35.5 C 4.300781 37.699219 6.199219 39.300781 8.398438 39.800781 C 11.898438 40.5 17.898438 41 24.5 41 C 31.101563 41 37.101563 40.5 40.601563 39.800781 C 42.800781 39.300781 44.699219 37.800781 45.101563 35.5 C 45.5 33 46 29.398438 46.101563 25 C 45.898438 20.5 45.398438 17 44.898438 14.5 Z M 19 32 L 19 18 L 31.199219 25 Z">
                  </path>
                </svg>
              </a>
            </div>
            
          </div>
        </div>
        
      </footer>
      
                                            
</template>
<script setup>

const emit = defineEmits(['update:modelValue', 'customEvent']);
function emitTopo(){
  emit('inicio');
}


</script>
<style lang="">

</style>