<template>
    <div class="min-window-height q-py-xl">
        <div class="column q-gutter-y-lg ">
            <div class="relative main-font title1 q-px-xl ">
                <div class="lets-word">
                    NEW ARRIVALS
                </div>
                <img class="absolute leaf-block" style="height:25px" src="../assets/custom_ellypse.png"/>
            </div>
            <div class="q-mt-xl row items-center justify-center">
                <div class="col row justify-center">
                    <ClotheComponent 
                    is-clothe 
                    image="categorie1.png"  
                    title="Hoodies & Sweetshirt"
                    />
                </div>
                <div class="col row justify-center">
                    <ClotheComponent 
                    is-clothe 
                    image="categorie2.png"  
                    title="Coats & Parkas"
                    />
                </div>
                <div class="col row justify-center">
                    <ClotheComponent 
                    is-clothe 
                    image="categorie3.png"
                    title="Tees & T-Shirt"
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
.leaf-block{
    left: 17%;
    top: 50%;
    z-index: 1;
}

.leaf-block2{
    left: 17%;
    top: 60%;
    z-index: 1;
}
</style>