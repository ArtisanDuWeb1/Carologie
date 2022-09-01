<script setup>
  import Index from './components/Index.vue'
</script>

<template>
  <div class="h-screen overflow-hidden relative">
    <div class="flex justify-between px-4 mt-3 absolute z-30 top-0 right-0 left-0">
      <i class="fas fa-info-circle fa-3x icon" data-toggle="modal" data-target="#exampleModal"></i>
    </div>
    <Index/>
  </div>
</template>

<style>
  .icon {
    position: relative;
    padding: 0.1em;
    border-radius: 25px;
    color: white;
    background-color: #dc3545;
    margin: 0 0.2em;
    cursor: pointer;
  }

  .icon:hover {
      color: #ddd;
      transform: scale(1.1);
      transition: all 0.2s;
  }
</style>
