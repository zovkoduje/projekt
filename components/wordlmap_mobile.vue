<template>
    <div class="relative mt-20 -mb-72 md:hidden">
     <div class="w-72 mx-auto" id="app">
       <transition-group name="fade" mode="out-in">
         <div :key="index" v-for="(item, index) in data" v-show="index === current">
           <h1 class="font-black text-2xl mb-4">{{ item.title }}</h1>
           <hr class="bg-blue-500 w-72 h-2 mb-4 rounded" />
           <p>{{ item.content }}</p>
         </div>
       </transition-group>
     </div>

     <img class="absolute  top-3/4 md:top-2/3 left-1/2 transform -translate-x-1/2 -translate-y-1/2" src="/imgs/spinner_world.png">
     <div class="relative mt-20 mb-96 image-container">
       <img class="mx-auto -mb-10 rotating-image" src="/imgs/spinner_2.png">
       <div class="flex justify-center p-0.5">
           <img class="rotating-image" src="/imgs/spinner_1.png">
           <img class="rotating-image" src="/imgs/spinner_3.png">
       </div>
     </div>
   </div>
   


</template>

<script>
export default {
 data() {
   return {
     current: 0,
     data: [
       {
         title: 'Estimation',
         content:
           'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum libero at ipsum ex! Ullam illum cupiditate deserunt consectetur excepturi recusandae sunt earum maxime ipsa, dignissimos facere, blanditiis, voluptatum necessitatibus inventore?',
       },
       {
         title: 'Specification',
         content:
         'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum libero at ipsum ex! Ullam illum cupiditate deserunt consectetur excepturi recusandae sunt earum maxime ipsa, dignissimos facere, blanditiis, voluptatum necessitatibus inventore?',
       },
       {
         title: 'Realisation',
         content:
         'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum libero at ipsum ex! Ullam illum cupiditate deserunt consectetur excepturi recusandae sunt earum maxime ipsa, dignissimos facere, blanditiis, voluptatum necessitatibus inventore?',
       },
     ],
   };
 },
 created() {
   this.startTransitionLoop();
 },
 methods: {
   startTransitionLoop() {
     setInterval(() => {
       this.current = (this.current + 1) % this.data.length;
     }, 5250); 
   },
 },
};

</script>

<style lang="scss" scoped>
.image-container {
 position: relative;
 animation: rotate 18s linear infinite;
 
 
 transform-origin: 50% 65%;
}



@keyframes rotate {
 0% {
   transform: rotate(0deg);
 }
 15%{
   transform: rotate(0deg);
 }
 30%{
   transform: rotate(120deg);
 }
 45%{
   transform: rotate(120deg);
 }
 60%{
   transform: rotate(240deg);
 }
 75%{
   transform: rotate(240deg);
 }
 90%{
   transform: rotate(360deg);
 }
 100% {
   transform: rotate(360deg);
 }
}
.fade-enter-active,
.fade-leave-active {
 transition: filter 5s;
}

.fade-enter,
.fade-leave-to {
 filter: blur(100px);
}

.fade-leave-active {
 position: absolute;
 top:0;
}

.fade-enter-to {
 filter: blur(0);
}




</style>