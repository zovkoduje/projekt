<template>
    <div class="relative flex items-center -rotate-90 gap-10">
        <div :style="{ color: textColor }" class="ml-2 text-xl font-semibold">
            {{ word }}
        </div>
        <hr class="w-1 h-full bg-black lg:w-1/2 lg:h-1 "/>
      
    </div>
  </template>
  
  <script>
  export default {
    props: {
      word: {
        type: String,
        required: true
      },
      textColor: {
      type: String,
      default: "black"
    }
    }
  }
  </script>
  
  <style scoped>
  /* Add any additional styling here */
  </style>
  