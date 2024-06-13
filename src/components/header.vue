<!-- eslint-disable vue/multi-word-component-names -->
<script setup lang="ts">
import { ref } from 'vue';
import logo from '@/components/icons/logo.vue'
import menuB from '@/components/icons/menu.vue'

let isMenuOpen = ref(false)

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value
}

defineExpose({
  isMenuOpen,
  toggleMenu
})
</script>

<template>
    <div class="bg-[#519DC8]">
    <header  class="flex h-20 text-white">
        <logo class="ml-2 flex"/>
        <h1 class="font-header-title, text-7xl ml-2">Student'Book</h1>
        <p class="ml-[700px] my-auto text-2xl">Se connecter</p>
        <button><menuB class="flex ml-[30px] h-10 mt-2" @click="toggleMenu"/></button>
    </header>

     <ul class="h-screen text-center absolute w-screen z-10 bg-[#519DC8]" v-show="isMenuOpen">
            <li  class="text-white text-2xl  hover:text-3xl hover:font-bold hover:text-black">Accueil</li>
            <li class="text-white text-2xl  hover:text-3xl hover:font-bold hover:text-black">Actualité</li>
            <li class="text-white text-2xl  hover:text-3xl hover:font-bold hover:text-black">À propos</li>
            <li class="text-white text-2xl  hover:text-3xl hover:font-bold hover:text-black">Newsletter</li>
     </ul>
</div>
</template>