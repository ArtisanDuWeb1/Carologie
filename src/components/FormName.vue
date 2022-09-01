<template>
    <div class="">
        <form >
            <div id="nom" class="row d-none">
                <div class="w-full">
                    <div class="flex justify-content-center">
                        <div class="w-full md:w-10/12 p-0">
                            <input type="text" id="tags1" name="nom" class="px-4 search-slt" placeholder="Nom de la personne...">
                        </div>
                        
                        <div class="w-full md:w-1/12 p-0">
                            <button type="submit"  class="bg-red-500 wrn-btn text-white hover:bg-red-600 transition-all easy-in">
                                <i class="fas fa-search"></i>
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </form>
    </div>
</template>

<script setup>
    
</script>

<style>
    #tags1{
        border-top-left-radius:50px;
        border-bottom-left-radius:50px;
    }
    
</style>