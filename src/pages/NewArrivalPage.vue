<template>
    <div class="min-window-height q-py-xl">
        <div class="column q-gutter-y-lg ">
            <div class="relative main-font title1 q-px-xl ">
                <div class="lets-word">
                    NEW ARRIVALS
                </div>
                <img class="absolute leaf-block" style="height:25px" src="../assets/custom_ellypse.png"/>
            </div>
            <div class="q-mt-xl row items-center justify-center gt-sm">
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
            <div class="q-mt-xl row items-center justify-center lt-md overflow-hidden">
                <q-carousel
                v-model="slide"
                transition-prev="slide-right"
                transition-next="slide-left"
                animated
                control-type="push"
                padding
                arrows
                infinite
                control-color="black"
                class="rounded-borders carousel-clothe"
                >
                    <q-carousel-slide 
                    v-for="(item,index) in datas"
                    :key="index"
                    :name="index" 
                    >
                        <ClotheComponent 
                        is-clothe 
                        :image="item.image"  
                        :title="item.title"
                        />
                    </q-carousel-slide>
            </q-carousel>
            </div> 
        </div>
    </div>
</template>

<script setup lang="ts">
import ClotheComponent from '../components/ClotheComponent.vue';
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel'
import { reactive, ref } from 'vue';

const datas = [
    {
        title:'Hoodies & Sweetshirt',
        image:'categorie1.png'
    },
    {
        title:'Coats & Parkas',
        image:'categorie2.png'
    },
    {
        title:'Tees & T-Shirt',
        image:'categorie3.png'
    }
]

const slide = ref(1)
</script>

<style>
.leaf-block{
    left: 40%;
    top: 45%;
    z-index: 1;
}

.leaf-block2{
    left: 60%;
    top: 45%;
    z-index: 1;
}
.carousel-clothe{
    height:500px
}
.relative{
    position: relative;
}
@media (min-width: 600px) {
    .carousel-clothe{
        height:600px
    }
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
}
</style>