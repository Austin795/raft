<script setup lang="ts">

import { ref } from 'vue'

const items = ref([{ koi: 'Kohaku', file:'koi_1.svg' }, 
                   { koi: 'Ki Utsuri', file: 'koi_2.svg' },
                   { koi: 'Tancho Showa', file: 'koi_3.svg' },
                   { koi: 'Kohaku', file: 'koi_4.svg' },
                   { koi: 'Tancho Showa', file: 'koi_5.svg' },
                   { koi: 'Kohaku', file: 'koi_6.svg' },
                   { koi: 'Kohaku', file: 'koi_7.svg' },
                   { koi: 'Kohaku', file: 'koi_8.svg' },
                   { koi: 'Hi Utsuri', file: 'koi_9.svg' },
                   { koi: 'Kohaku', file: 'koi_10.svg' },
                  ])

</script>

<template>
  <div class="static grid grid-cols-5 gap-4">
      <button class="border-transparent p-5" v-for="(item) in items">
        <a class="h-50 w-25">
          <img :src="`../src/assets/${item.file}`" />  
        </a>
        <br>
        <div class="static bottom-0 left-0">
          <h1 class="font-bold font-mono font-black hover:italic">{{ `${item.koi}` }}</h1>
        </div>
      </button>
  </div>
</template>

<style scoped>
</style>
