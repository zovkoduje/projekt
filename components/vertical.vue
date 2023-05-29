<template>
    <div class="hidden @screen md:flex w-1 h-screen bg-gray-600 absolute left-20 -top-10 ">
      <p :class="['-rotate-90', textColor, 'text-4xl',' absolute -bottom-60 -left-28']">{{ text }}</p>
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

    },
    computed: {
      textColor() {
        return this.color;
      },
      textSize() {
        return this.size;
      },
    },
  };
  </script>
  