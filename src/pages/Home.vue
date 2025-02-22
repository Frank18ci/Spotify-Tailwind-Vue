<template>
 <div class="2xl:w-[87%] w-[76%] bg-dark overflow-scroll">
      <div class="flex justify-between px-10 py-4 bg-dark-darker sticky top-0 z-20">
        <div class="space-x-2">
          <button class="p-[.2rem] bg-dark-light rounded-full">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6">
              <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 19.5 8.25 12l7.5-7.5" />
            </svg>
          </button>
          <button class="p-[.2rem] bg-dark-light rounded-full">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6">
              <path stroke-linecap="round" stroke-linejoin="round" d="m8.25 4.5 7.5 7.5-7.5 7.5" />
            </svg>
          </button>
        </div>
        <div class="flex gap-x-2">
          <button class="button-bordered"> 
            Mejora tu cuenta
          </button>
          <button class="h-8 flex items-center gap-x-2 pe-3 ps-[.15rem]   rounded-full  text-sm font-semibold bg-neutral-800 hover:bg-neutral-900"> 
            <div class="size-7 rounded-full overflow-hidden">
              <img src="../../public/images/avatar.jpeg" alt="">
            </div>
            <div>
              Jairo
            </div>
            <div>
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-4">
                <path stroke-linecap="round" stroke-linejoin="round" d="m19.5 8.25-7.5 7.5-7.5-7.5" />
              </svg>
            </div>
          </button>
        </div>
      </div>
      <div class="px-10 pt-10 pb-28">
       <div>
        <div class="flex justify-between">
          <h2 ><a href="" class="text-light-primary text-2xl font-bold hover:underline">Escuchados recientemente</a></h2>
          <button class="text-light-secondary font-bold text-sm hover:underline cursor-pointer">Mostrar todos</button>
        </div>
        <div class="mt-8 grid grid-rows-1 lg:grid-cols-4 xl:grid-cols-5 sm:grid-cols-3 2xl:grid-cols-8  3xl:grid-cols-8 gap-x-5">
          
          <Tile
            title="Sergio Sacoto"
            sub-title="Artista"
            image="/images/sacoto.jpeg"
          />

          <Tile
            title="Enanitos Verdes"
            sub-title="Artista"
            image="/images/enanitos.jpeg"
          />
          <Tile
            title="00s Rock Anthems"
            sub-title="These songs rocked the 00s. Cover: Green Day"
            image="/images/rock.jpeg"
            shape="square"
          />

          
        </div>

        
       </div>
      </div>
    </div>

</template>
<script setup>
    import Tile from './src/components/Tile.vue'
</script>