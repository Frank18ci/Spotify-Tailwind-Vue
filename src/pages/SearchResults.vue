<template>
    <div class="2xl:w-[87%] w-[76%] bg-dark overflow-scroll">
         <div class="flex justify-between px-10 py-4 bg-dark-darker sticky top-0 z-20">
            <div class="flex gap-x-5 items-center">
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
                <div class="relative">
                    <input class="outline-none rounded-full h-10 w-72 ps-10 pe-5 bg-light-primary text-dark"
                         type="text" name="" id=""
                         placeholder="¿Que quieres escuchar?">
                         <div class="absolute text-dark top-2 left-3">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6">
                                <path stroke-linecap="round" stroke-linejoin="round" d="m21 21-5.197-5.197m0 0A7.5 7.5 0 1 0 5.196 5.196a7.5 7.5 0 0 0 10.607 10.607Z" />
                            </svg>
                         </div>
                </div>    
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
         <div>
            
         </div>
         <div class="px-10 pt-8 pb-28">
            <div class="flex gap-x-2 my-4">
                <div class="bg-light-primary text-dark font-semibold rounded-full px-3 py-1">
                    Todo
                </div>
                <div class="bg-dark-light rounded-full px-3 py-1">
                    Artista
                </div>
                <div class="bg-dark-light rounded-full px-3 py-1">
                    Género
                </div>
                <div class="bg-dark-light rounded-full px-3 py-1">
                    Albunes
                </div>
            </div>
          <div class="flex flex-col lg:flex-row gap-x-5">
                <div class="w-full lg:w-2/5">
                    <div class="flex justify-between">
                        <h2 class="text-light-primary text-2xl font-bold">Resultado Principal</h2>
                    </div>
                    <div class="p-4 bg-dark-light mt-5 rounded space-y-3">
                        <div>
                            <img class="rounded-full w-28" src="/images/sacoto.jpeg" alt="">
                        </div>
                        <div>
                            <h2 class="text-light-primary text-3xl font-bold">Sergio Sacoto</h2>
                        </div>
                        <div class="flex">
                            <div class="bg-dark font-semibold rounded-full px-3 py-1">
                                Artista
                            </div>
                        </div>
                    </div>
                </div>
                <div class="w-full lg:w-3/5">
                    <div class="flex justify-between">
                        <h2 class="text-light-primary mt-3 text-2xl font-bold ">Canciones</h2>
                    </div>
                    <div>
                        <div class="group flex justify-between items-center hover:bg-dark-light rounded  p-2">
                            <div class="flex gap-x-4 ">
                                <div class="relative">
                                    <img class="w-12 group-hover:brightness-50" src="/images/sacoto.jpeg" alt="">
                                    <svg class="size-6 absolute top-[30%] left-[30%] transition opacity-0 group-hover:opacity-100" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" >
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M5.25 5.653c0-.856.917-1.398 1.667-.986l11.54 6.347a1.125 1.125 0 0 1 0 1.972l-11.54 6.347a1.125 1.125 0 0 1-1.667-.986V5.653Z" />
                                    </svg>
                                </div>
                                <div>
                                    <h3 class="font-semibold">Al Borde (en vivo)</h3>
                                    <div class="text-sm hover:underline"><a href="#">Sergio Sacoto</a></div>
                                </div>
                            </div>
                            <div class="flex items-center gap-x-3">
                                <div class="px-5 flex items-center">
                                    <Like :like="true" />
                                </div>
                                <div class="text-light-secondary">
                                    4:39
                                </div>
                                <div>
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6">
                                     <path stroke-linecap="round" stroke-linejoin="round" d="M6.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0ZM12.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0ZM18.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0Z" />
                                    </svg>
                                </div>
                            </div>
                        </div>
                        <div class="group flex justify-between items-center hover:bg-dark-light rounded  p-2">
                            <div class="flex gap-x-4 ">
                                <div class="relative">
                                    <img class="w-12 group-hover:brightness-50" src="/images/sacoto.jpeg" alt="">
                                    <svg class="size-6 absolute top-[30%] left-[30%] transition opacity-0 group-hover:opacity-100" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" >
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M5.25 5.653c0-.856.917-1.398 1.667-.986l11.54 6.347a1.125 1.125 0 0 1 0 1.972l-11.54 6.347a1.125 1.125 0 0 1-1.667-.986V5.653Z" />
                                    </svg>
                                </div>
                                <div>
                                    <h3 class="font-semibold">Al Borde (en vivo)</h3>
                                    <div class="text-sm hover:underline"><a href="#">Sergio Sacoto</a></div>
                                </div>
                            </div>
                            <div class="flex items-center gap-x-3">
                                <div class="px-5 flex items-center">
                                    <Like :like="true" />
                                </div>
                                <div class="text-light-secondary">
                                    4:39
                                </div>
                                <div>
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6">
                                     <path stroke-linecap="round" stroke-linejoin="round" d="M6.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0ZM12.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0ZM18.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0Z" />
                                    </svg>
                                </div>
                            </div>
                        </div>
                        <div class="group flex justify-between items-center hover:bg-dark-light rounded  p-2">
                            <div class="flex gap-x-4 ">
                                <div class="relative">
                                    <img class="w-12 group-hover:brightness-50" src="/images/sacoto.jpeg" alt="">
                                    <svg class="size-6 absolute top-[30%] left-[30%] transition opacity-0 group-hover:opacity-100" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" >
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M5.25 5.653c0-.856.917-1.398 1.667-.986l11.54 6.347a1.125 1.125 0 0 1 0 1.972l-11.54 6.347a1.125 1.125 0 0 1-1.667-.986V5.653Z" />
                                    </svg>
                                </div>
                                <div>
                                    <h3 class="font-semibold">Al Borde (en vivo)</h3>
                                    <div class="text-sm hover:underline"><a href="#">Sergio Sacoto</a></div>
                                </div>
                            </div>
                            <div class="flex items-center gap-x-3">
                                <div class="px-5 flex items-center">
                                    <Like :like="true" />
                                </div>
                                <div class="text-light-secondary">
                                    4:39
                                </div>
                                <div>
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6">
                                     <path stroke-linecap="round" stroke-linejoin="round" d="M6.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0ZM12.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0ZM18.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0Z" />
                                    </svg>
                                </div>
                            </div>
                        </div>
                        <div class="group flex justify-between items-center hover:bg-dark-light rounded  p-2">
                            <div class="flex gap-x-4 ">
                                <div class="relative">
                                    <img class="w-12 group-hover:brightness-50" src="/images/sacoto.jpeg" alt="">
                                    <svg class="size-6 absolute top-[30%] left-[30%] transition opacity-0 group-hover:opacity-100" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" >
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M5.25 5.653c0-.856.917-1.398 1.667-.986l11.54 6.347a1.125 1.125 0 0 1 0 1.972l-11.54 6.347a1.125 1.125 0 0 1-1.667-.986V5.653Z" />
                                    </svg>
                                </div>
                                <div>
                                    <h3 class="font-semibold">Al Borde (en vivo)</h3>
                                    <div class="text-sm hover:underline"><a href="#">Sergio Sacoto</a></div>
                                </div>
                            </div>
                            <div class="flex items-center gap-x-3">
                                <div class="px-5 flex items-center">
                                    <Like :like="true" />
                                </div>
                                <div class="text-light-secondary">
                                    4:39
                                </div>
                                <div>
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6">
                                     <path stroke-linecap="round" stroke-linejoin="round" d="M6.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0ZM12.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0ZM18.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0Z" />
                                    </svg>
                                </div>
                            </div>
                        </div>
                        
                    </div>
                </div>
          </div>
        
         </div>
       </div>
   
   </template>
   <script setup>
        import Like from '../components/Like.vue';
        
   </script>