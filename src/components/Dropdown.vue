<template>
        <div class="absolute z-10 w-55 flex flex-col p-1 bg-dark-light text-sm rounded shadow">
            
            <button  v-for="item in items" class="group relative flex justify-between items-center p-3 text-start hover:bg-dark-lighter cursor-pointer rounded">
              {{item.title}}
              <div>
                <ArrowTopRightOnSquare v-if="item.icon === 'ArrowTopRightOnSquare'" />
                <ChevronRight v-if="item.icon === 'ChevronRight'" />
              </div>

              <div class="absolute left-[100%] top-0">
                <Dropdown 
                    class="opacity-0 group-hover:opacity-100 transition"
                    v-if="item.items !== null" 
                    :items="item.items" />
              </div>
            </button>
          </div>
</template>

<script setup>
    import ArrowTopRightOnSquare from '../icons/ArrowTopRightOnSquare.vue';
    import ChevronRight from '../icons/ChevronRight.vue';
    defineProps({
        items: Array,
    })
</script>