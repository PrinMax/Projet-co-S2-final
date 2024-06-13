<!-- eslint-disable vue/multi-word-component-names -->
<script setup lang="ts">
import logo from './icons/logo.vue';
import Facebook from './icons/Facebook.vue';
import insta from './icons/insta.vue';
import twitter from './icons/twitter.vue';
</script>
<template>
    <div>
        <footer class="bg-[#519DC8]">
            <div class="flex h-20 text-white">
                <logo class="ml-2 flex"/>
                <div>
                    <p>À propos</p>
                </div>
                <div class="flex ml-[30px] h-10 mt-2">
                    <Facebook class="ml-2"/>
                    <insta class="ml-2"/>
                    <twitter class="ml-2"/>
                </div>
            </div>
        </footer>
    </div>
</template>