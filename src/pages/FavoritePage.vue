<template>
    <div class="min-window-height q-py-md-xl q-py-none">
        <div class="column q-gutter-y-lg ">
            <div class="relative main-font title1 q-px-xl ">
                <div class="lets-word">
                    YOUNG'S FAVORITE
                </div>
                <img class="absolute leaf-block2" style="height:20px" src="../assets/custom_ellypse.png"/>
            </div>
            <div class="q-mt-xl row items-center justify-center">
                <div
                v-for="item in datas"
               :key="item.title" 
                class="col-12 col-md-6 row justify-center items-center"
               >
                    <ClotheComponent 
                    :image="item.image" 
                    :title="item.title"
                    />
                </div>
            </div> 
        </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import ClotheComponent from '../components/ClotheComponent.vue';

const datas = [
    {
        title:'Trending on instagram',
        image:'favorite1.png'
    },
    {
        title:'Hoodies & Sweetshirt',
        image:'favorite2.png'
    }
]

const slide = ref(1)
</script>

<style>

</style>