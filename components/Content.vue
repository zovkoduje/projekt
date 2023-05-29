<template>
  <div class="flex flex-col-reverse justify-center items-center md:flex-row">
    <div :class="[textClass, 'pt-10 pl-10 w-full sm:w-1/2']">
      <h1 :style="{ color: textColor }" class="font-black text-6xl mb-10 text-center md:text-left">{{ title }}</h1>
      <p :style="{ color: textColor }">{{ textContent}}</p>
    </div>
    <div :class="[imageClass, 'p-10']">
      <img :src="imageSrc" />
    </div>
  </div>
</template>
  
  <script>
  export default {
    props: {
      title: {
        type: String,
        required: true
      },
      textContent: {
        type: String,
        required: true
      },
      imageSrc: {
        type: String,
        required: true
      },
      imageOnLeft: {
        type: Boolean,
        default: true
      },
      textColor: {
        type: String,
        default: "#343A40"
      }
    },
    computed: {
      textClass() {
        return this.imageOnLeft ? 'order-2' : '';
      },
      imageClass() {
        return this.imageOnLeft ? 'order-1' : '';
      }
    }
  };
  </script>
<style>
</style>  