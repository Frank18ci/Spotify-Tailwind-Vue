<template>
    <div :class="background" class="flex flex-col justify-between  h-48 pt-5 ps-4 overflow-hidden rounded">
        <h2 class="text-2xl font-bold">{{ name }}</h2>
        <div class="flex justify-end">
            <img class="-mr-5 -mb-3 w-24 rotate-[30deg]" v-bind:src="image" alt="">
        </div>
    </div>            
</template>
<script setup>
defineProps({
    name: String,
    image: String,
    background: String
})
</script>