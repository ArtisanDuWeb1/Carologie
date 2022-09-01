<template>
    <div>
        <section class="search-sec">
            <form @submit.prevent="">
                <div class="flex flex-row justify-center flex-wrap">
                    <div class="w-full md:w-2/12 p-0">
                        <input type="text" id="oki" name="num" class="search-slt px-2 rounded-full" placeholder="N°..." required>
                    </div>
                    <div class="w-full md:w-4/12 p-0">
                        <input type="text" name="rue" id="tags" class="search-slt px-2" placeholder="Rue..." required>
                    </div>
                    <div class="w-full md:w-2/12 p-0">
                        <input type="number" class="search-slt px-2" value="1740" name="dateIn" id="dateIn" required>
                    </div>
                    <div class="w-full md:w-2/12 p-0">
                        <input type="number" class="search-slt px-2" value="1876" min="" name="dateOut" id="dateOut" required>
                    </div>
                    <div class="w-full md:w-1/12 p-0">
                        <button type="submit"  class="bg-red-500 wrn-btn text-white hover:bg-red-600 transition-all easy-in">
                            <i class="fas fa-search"></i>
                        </button>
                    </div>
                </div>
            </form>
        </section>
    </div>
</template>

<script setup>

</script>

<style>
    .search-slt{
        display: block;
        width: 100%;
        font-size: 1.8rem;
        font-weight: 800;
        line-height: 1.5;
        color: #55595c;
        background-color: #fff;
        background-image: none;
        border: 1px solid #ccc;
        height: calc(4rem + 4px) !important;
        border-radius:0;
    }
    #oki{
        border-top-left-radius:50px;
        border-bottom-left-radius:50px;
    }
    .wrn-btn{
        width: 100%;
        font-size: 16px;
        font-weight: 400;
        text-transform: capitalize;
        height: calc(4rem + 4px) !important;
        border-radius:0;
        border-top-right-radius:50px;
        border-bottom-right-radius:50px;
    }
</style>