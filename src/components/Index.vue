<template>
  <div class="h-full bg-red-400 index relative">
    <div class="old_style w-full h-full"></div>
    <div class="flex flex-col justify-center items-center h-[92%]">
      <div class="relative z-20">
        <div class="flex flex-row text-center justify-center">
          <h1 class="title">Découvrez qui habitait à Charleville</h1>
        </div>
        <div class="flex flex-row text-center justify-center">
          <span class="date">ENTRE 1739 ET 1876</span>
        </div>
        <component :is="currentForm ? Form : FormName" class="mt-12"></component>
        <div class="w-full flex justify-center mt-12">
          <button @click="currentForm = !currentForm" class="bg-red-500 px-6 py-3 text-xl text-white font-bold rounded-full hover:bg-red-600 transition-all easy-in">
            {{currentForm ? 'Rechercher par nom' : 'Rechercher par adresse'}}
          </button>
        </div>
      </div>  
    </div>
    <div class="w-full h-[8%] bg-red-500 relative ">
      <div class="flex items-center justify-around absolute w-full -top-[50px]">
        <div class="col-2 part_col">
            <div class="rounded-full bg-white p-3 overflow-hidden border-red-500 border-2">
              <img class="h-[70px] w-[70px]" src="img/cci.jpg" alt="">
            </div>
        </div>
        <div class="col-2 part_col">
            <div class="rounded-full bg-white p-3 overflow-hidden border-red-500 border-2">
              <img class="h-[70px] w-[70px]" src="img/rimbaudtech.jpg" alt="">
            </div>
        </div>
        <div class="col-2 part_col">
            <div class="rounded-full bg-white p-3 overflow-hidden border-red-500 border-2">
              <img class="h-[70px] w-[70px]" src="img/simplon.png" alt="">
            </div>
        </div>
        <div class="rounded-full bg-white p-3 overflow-hidden border-red-500 border-2">
            <div class="part hvr-pulse-grow">
              <img class="h-[70px] w-[70px]" src="img/hackardennes.svg" alt="">
            </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  import Form from './Form.vue'
  import FormName from './FormName.vue'
  import { ref } from 'vue'

  const currentForm = ref(true)

</script>

<style>
  .index {
    background-image: url(img/ducale.png);
    background-repeat: no-repeat;
    background-size: cover;
  }

  .old_style {
    position: absolute;
    background-image: url('../img/degueu2.gif');
    background-repeat: no-repeat;
    background-size: cover;
    opacity: 0.2;
    margin-top: -2em;
  }

  .title {
    text-align: center;
    font-family: 'Parisienne', cursive;
    font-size: 6em;
    font-weight: 900;
    line-height: 1.4em;
    color: white;
    word-spacing: 0.2em;
    text-shadow: #dc3545 5px 5px;
  }

  .date {
    text-align: center;
    font-size: 2em;
    font-weight: 700;
    color: white;
    letter-spacing: 0.05em;
    word-spacing: 0.1em;
  }
</style>