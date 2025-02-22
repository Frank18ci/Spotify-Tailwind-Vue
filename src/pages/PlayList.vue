<template>
    <div class="2xl:w-[87%] w-[76%] bg-dark overflow-scroll">
        <div class="flex justify-between px-10 py-4 bg-dark-darker sticky top-0 z-20">
            <div class="space-x-2">
                <button class="p-[.2rem] bg-dark-light rounded-full">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="size-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 19.5 8.25 12l7.5-7.5" />
                    </svg>
                </button>
                <button class="p-[.2rem] bg-dark-light rounded-full">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="size-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="m8.25 4.5 7.5 7.5-7.5 7.5" />
                    </svg>
                </button>
            </div>
            <div class="flex gap-x-2">
                <button class="button-bordered">
                    Mejora tu cuenta
                </button>
                <button
                    class="h-8 flex items-center gap-x-2 pe-3 ps-[.15rem]   rounded-full  text-sm font-semibold bg-neutral-800 hover:bg-neutral-900">
                    <div class="size-7 rounded-full overflow-hidden">
                        <img src="../../public/images/avatar.jpeg" alt="">
                    </div>
                    <div>
                        Jairo
                    </div>
                    <div>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor" class="size-4">
                            <path stroke-linecap="round" stroke-linejoin="round" d="m19.5 8.25-7.5 7.5-7.5-7.5" />
                        </svg>
                    </div>
                </button>
            </div>
        </div>

        <div class="flex from-blue-400 to-blue-900 bg-gradient-to-b pt-5 pb-7">
            <div class="w-1/4">
                <div class="size-48 object-cover mx-auto mt-4 overflow-hidden rounded-full ">
                    <img class="w-full h-full object-cover" src="/images/theweeknd.jpg" alt="">
                </div>
            </div>
            <div class="w-3/4 pt-20 space-y-4">
                <div class="sm:text-5xl xl:text-7xl font-bold ">The Weeknd</div>
                <div class="ms-2">140.140.200 oyentes mensuales</div>
            </div>
        </div>
        <div class="from-blue-950 to-30% to-dark bg-gradient-to-b">
            <div class="flex gap-x-5 items-center px-7 py-5">
                <div
                    class="text-dark-darker bg-green-primary rounded-full flex justify-center p-3 cursor-pointer hover:scale-105 transition hover:bg-green-secondary">
                    <button class="cursor-pointer">
                        <svg class="size-8" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24"
                            stroke-width="1.5" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M5.25 5.653c0-.856.917-1.398 1.667-.986l11.54 6.347a1.125 1.125 0 0 1 0 1.972l-11.54 6.347a1.125 1.125 0 0 1-1.667-.986V5.653Z" />
                        </svg>
                    </button>
                </div>
                <div>
                    <button
                        class="border rounded px-4 py-1 uppercase  cursor-pointer tracking-widest font-semibold text-sm">Siguiendo</button>
                </div>
                <div>
                    <svg class="size-10 hover:text-light-primary text-light-secondary cursor-pointer"
                        xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="M6.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0ZM12.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0ZM18.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0Z" />
                    </svg>
                </div>
            </div>
            <div class=" px-7 pb-28">
                <h2 class="text-2xl font-bold">Populares</h2>
                <div class="mt-3">
                    <Track  
                    :track-numer="1"
                    image="/images/soda.jpeg"
                    track-name="Al border (en vivo)"
                    duration="4:58"
                    :like="true"
                     />
                     <Track  
                    :track-numer="2"
                    image="/images/sacoto.jpeg"
                    track-name="Lamento Boliano"
                    duration="3:58"
                    :like="false"
                     />
                     <Track  
                    :track-numer="3"
                    image="/images/nickel.jpeg"
                    track-name="La muralla verde"
                    duration="5:02"
                    :like="true"
                     />
                     <Track  
                    :track-numer="4"
                    image="/images/soda.jpeg"
                    track-name="Tu carcel (en vivo)"
                    duration="2:58"
                    :like="false"
                     />
                     <Track  
                    :track-numer="5"
                    image="/images/nickel.jpeg"
                    track-name="Mariposas"
                    duration="4:58"
                    :like="true"
                     />
                </div>
                <div class="ml-5 mt-4">
                    <a class="font-semibold text-light-secondary hover:text-light-primary" href="#">See more</a>
                </div>
            </div>
        </div>


    </div>

</template>
<script setup>
import Track from '../components/Track.vue';
import Tile from './src/components/Tile.vue'
</script>