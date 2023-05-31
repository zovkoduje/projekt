<template>
    <div class="md:hidden flex relative justify-center">
      <p :class="[textColor, 'text-2xl my-6 ']">{{ text }}</p>
      <div :style="{ backgroundColor: backgroundColor }" class="h-1 rounded w-20 absolute top-10 right-0"></div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      text: {
        type: String,
        required: true,
      },
      color: {
        type: String,
        default: '#343A40',
      },
      backgroundColor: {
        type: String,
        default: '#343A40',
      },
    },
    computed: {
      textColor() {
        return this.color;
      },
    },
  };
  </script>
  