<template>
    <div class="min-window-height q-py-xl">
        <div class="column q-gutter-y-lg ">
            <div class="relative main-font title1 q-px-xl ">
                <div class="lets-word">
                    Youngs'favorite
                </div>
                <img class="absolute leaf-block2" style="height:20px" src="../assets/custom_ellypse.png"/>
            </div>
            <div class="q-mt-xl row items-center justify-center">
                <div class="col row justify-center">
                    <ClotheComponent 
                    image="favorite1.png" 
                    title="Trending on instagram"
                    />
                </div>
                <div class="col row justify-center">
                    <ClotheComponent 
                    image="favorite2.png" 
                    title="Hoodies & Sweetshirt"
                    />
                </div>
            </div> 
        </div>
    </div>
</template>

<script setup lang="ts">
import ClotheComponent from '../components/ClotheComponent.vue';


</script>

<style>

</style>