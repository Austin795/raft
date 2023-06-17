<script>

</script>

<template>
  <div class="static grid grid-cols-5 gap-4">
    <li v-for="(item, index) in items">
  	    {{ index }} - {{ item.message }}
	  </li>
    <!-- <button class="border-transparent p-5" v-for="n in 10" :key="n">
      <a class="h-50 w-25">
        <img :src="`../src/assets/koi_${n}.svg`" />  
      </a>
      <br>
      <div class="static bottom-0 left-0">
        <h1 class="font-bold font-mono font-black hover:italic">{{ `Tancho Showa ${n}` }}</h1>
      </div>
    </button>-->
  </div>
</template>

<style scoped>
</style>


