<template>
 <div class="group flex justify-between items-center hover:bg-dark-light rounded  p-2">
                            <div class="w-1/3 flex gap-x-4 items-center">
                                <div class="relative">
                                    <div class="group-hover:opacity-0">{{ trackNumer }}</div>
                                    <svg class="size-6 absolute top-[5%] -left-1 transition opacity-0 group-hover:opacity-100" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" >
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M5.25 5.653c0-.856.917-1.398 1.667-.986l11.54 6.347a1.125 1.125 0 0 1 0 1.972l-11.54 6.347a1.125 1.125 0 0 1-1.667-.986V5.653Z" />
                                    </svg>
                                </div>
                                <div class="relative">
                                    <img class="w-12 group-hover:brightness-50" v-bind:src="image" alt="">
                                    
                                </div>
                                <div>
                                    <h3 class="font-semibold">{{ trackName }}</h3>
                                </div>
                            </div>
                            <div class="text-light-secondary group-hover:text-light-primary">
                                120.343.245
                            </div>
                            <div class="flex items-center gap-x-3">
                                <div class="px-5 flex items-center">
                                    <Like :like="like" />
                                </div>
                                <div class="text-light-secondary">
                                    {{ duration }}
                                </div>
                                <div>
                                    <svg class="size-6 opacity-0 group-hover:opacity-100 transition" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" >
                                     <path stroke-linecap="round" stroke-linejoin="round" d="M6.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0ZM12.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0ZM18.75 12a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0Z" />
                                    </svg>
                                </div>
                            </div>
                        </div>
</template>
<script setup>
    import Like from './Like.vue';
    defineProps({
        trackNumer: Number,
        image: String,
        trackName: String,
        duration: String,
        like: Boolean
    })
</script>