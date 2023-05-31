<template>

    <nav class="hidden md:flex bg-transparent pt-20 pr-20 justify-end">
        <ul class="flex gap-6 items-center">
            <li class="text-xl"><NuxtLink to="/">Way we do it</NuxtLink></li>
            <li class="text-xl"><NuxtLink to="/">Partners</NuxtLink></li>
            <button class="h-16 flex-row justify-center items-center flex gap-11.14 bg-gray-700 rounded-3xl text-white">
                <span class="text-xl font-semibold text-white mx-5">Let's chat</span>
            </button>
        </ul>
    </nav>

    <div class="md:hidden flex ">
        <input type="checkbox" id="toggle" class="hidden" />
        <label for="toggle" class="block cursor-pointer p-4">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor"
                stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6">
                <path d="M3 12h18M3 6h18M3 18h18"></path>
            </svg>
        </label>
        <div class="hidden bg-transparent p-4" id="menu">
            <ul class="flex flex-col gap-4">
                <li class="text-xl"><NuxtLink to="/">Way we do it</NuxtLink></li>
                <li class="text-xl"><NuxtLink to="/">Partners</NuxtLink></li>
                <button class="h-16 w-48 flex-row justify-center items-center flex gap-11.14 bg-gray-700 rounded-lg text-white">
                    <span class="text-xl font-semibold text-white">Let's chat</span>
                </button>
            </ul>
        </div>
    </div>

</template>

<script setup>

</script>

<style scoped>
 /* Hide the menu initially */
 #menu {
        display: none;
    }

    /* Show the menu when the checkbox is checked */
    #toggle:checked ~ #menu {
        display: block;
    }

    /* Hide the original navigation on small screens */
    @media (max-width: 767px) {
        nav.hidden {
            display: none;
        }
    }
</style>