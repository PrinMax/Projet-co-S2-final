<!-- eslint-disable vue/multi-word-component-names -->
<script setup lang="ts">
const font = 'font-body';
import flèche from '@/components/icons/flèche.vue'
</script>

<template>
  <div class="title">
  <body class="bg-[#DDDDDD]">
  <div style="width: 100%; ">
    <div style="z-index: 1;">
      <img src="C:\Users\Max88\Desktop\ProjetS2\src\components\img\image 1 (1) 1.webp" alt="image d'accueil">
    </div>
    <div style="position: absolute;top: 300px;width: 650px; height: 400px; z-index: 2; font-size: 200%; margin-left: 450px;">
      <div class="font-body-text">
      <p class="text-white">Étudiants, améliorez votre veille et simplifiez vos études avec Student’Book</p>
    </div>
    </div>
  </div>
  <h1 class="underline underline-offset-1 text-xl">À la une :</h1>

<body class="bg-gray-100 flex items-center justify-center min-h-screen">

    <div class="overflow-x-auto flex space-x-4 p-4 snap-x snap-mandatory">
        <div class="min-w-full flex-shrink-0 snap-center">
            <div class="bg-white rounded-lg shadow-lg p-6 flex">
                <h2 class="text-2xl font-bold underline-offset-1 ml-[70px] place-content-center"  >Intelligence artificielle : Sam Altman réintègre le conseil d'administration d'OpenAI</h2>
                <img src="C:\Users\Max88\Desktop\ProjetS2\src\components\img\image 2.webp" alt="image du 1er article" width="10%" height="10%" class="ml-[70px]">
            </div>
        </div>
        <div class="min-w-full flex-shrink-0 snap-center">
            <div class="bg-white rounded-lg shadow-lg p-6 flex">
                <h2 class="text-2xl font-bold underline-offset-1 ml-[70px] place-content-center">L'intelligence artificielle menace-t-elle l'environnement ?</h2>
                <img src="C:\Users\Max88\Desktop\ProjetS2\src\components\img\image 3.webp" alt="image du 2eme article" width="10%" height="10%" class="ml-[150px]">
            </div>
        </div>
        <div class="min-w-full flex-shrink-0 snap-center">
            <div class="bg-white rounded-lg shadow-lg p-6 flex">
                <h2 class="text-2xl font-bold underline-offset-1 ml-[70px] place-content-center">Qu'est-ce que la Green IT ?</h2>
                <img src="C:\Users\Max88\Desktop\ProjetS2\src\components\img\image 4.webp" alt="image du 3eme article" width="10%" height="10%" class="ml-[400px]">
            </div>
        </div>
                <div class="min-w-full flex-shrink-0 snap-center">
            <div class="bg-white rounded-lg shadow-lg p-6 flex">
                <h2 class="text-2xl font-bold underline-offset-1 ml-[70px] place-content-center">Selon IBM, l'informatique quantique pourrait détruire la cybersécurité des pays</h2>
                <img src="C:\Users\Max88\Desktop\ProjetS2\src\components\img\image 5.webp" alt="image du 4eme article" width="10%" height="10%" class="ml-[250px]">
            </div>
        </div>
    </div>
<div>
  <p class="bg-[#C2E9FF] line-clamp-3">Avec Student’Book retrouvez toutes les actualités regroupées en un seul endroit et sur différents domaines afin de parfaire votre veille.</p>
</div>
</body>

  </body>
  </div>
</template>
