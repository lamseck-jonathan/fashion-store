<template>
    <div class="column items-center">
        <q-card style="background:#F4F6F5;" class="row overflow-hidden hero-container q-mt-lg rounded">
            <div class="column col-12 col-md-6 q-pl-xl q-pt-xl q-gutter-y-sm">
                <div class="main-font hero-text q-my-sm">
                    <span class="text-block bg-white"></span>
                    <div class="lets-word">
                        LET’S
                    </div>
                </div>
                <div class="main-font hero-text q-my-sm">
                    EXPLORE </div>
                <div class="main-font hero-text">
                    <span class="text-block2 bg-yellow-theme"></span>
                    <div class="lets-word">
                        UNIQUE
                    </div>
                </div>
                <div class="main-font hero-text">
                    CLOTHES.
                </div>
                <div class="main-font q-pb-md hero-sub-title">
                    Live for Influential and Innovative fashion!
                </div>
                <div class="row items-center q-gutter-none q-gutter-md-md">
                    <img style="height:25px" src="../assets/custom_ellypse.png"/>
                    <q-btn no-caps class="q-px-lg" style="height:50px" color="black" label="Shop Now"/>
                </div>
            </div>
            <div class="relative row col-12 col-md-6">
                <div class="relative">
                    <img class="star1" src="../assets/star.png"/>
                </div>
                <div class="relative">
                    <img class="star2" src="../assets/star.png"/>
                </div>
                <div class="relative">
                    <img class="star3" src="../assets/star.png"/>
                </div>
                <div class="relative">
                    <img class="star4" src="../assets/star.png"/>
                </div>
                <img class="hero-women" src="../assets/women2.png"/>
             </div>
        </q-card>
        <carousel
        style="height:100px"
        class="row items-center justify-between bg-yellow-theme brands q-mt-xl full-width" 
        :autoplay="100"
        :settings="settings"
        :breakpoints="breakpoints"
        :wrap-around="true"
        :transition="2000"
        >
            <slide v-for="brand in 12" :key="brand">
                <img class="carousel__item" style="width:100px" :src="'brand'+brand+'.png'"/>
            </slide>
        </carousel>
    </div>
    
</template>

<script setup lang="ts">
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel'
import { reactive } from 'vue';
const settings = reactive({
    itemsToShow: 3,
    snapAlign: 'center',
})

const breakpoints= reactive({
      // 700px and up
      600: {
        itemsToShow:6,
        snapAlign: 'center',
      }
})
</script>

<style>

.hero-container{
    width:90%;
    height: fit-content;
}
.hero-women{
    margin-left: 10%;
    width:300px;
}
.hero-sub-title{
    font-weight: 400;
    font-size: 20px;
    line-height: 48px;
    letter-spacing: -0.05em;
}
.text-block{
    position: absolute;
    width: 250px;
    height: 75px;
    content: '';
    z-index: 1;
    transform: rotate(-2deg);
    left: 3%;
}
.text-block2{
    position: absolute;
    width: 275px;
    height: 75px;
    content: '';
    z-index: 1;
    transform: rotate(-2deg);
    left: 3%;
}
.text-block3{
    position: absolute;
    width: 250px;
    height: 75px;
    content: '';
    z-index: 1;
    transform: rotate(-2deg);
    left: -25%;
    top:-5px;
}
.relative{
    position: relative;
}
.lets-word{
    position: relative;
    z-index: 10;
}
.star1{
    position: absolute;
    left:100px;
    top:10px;
}
.star2{
    position: absolute;
    top:190px;
    left:15px;
}
.star3{
    position: absolute;
    top:250px;
    left: 280px;
}
.star4{
    position: absolute;
    top:80px;
    left: 260px;
}
.star5{
    position: absolute;
    top:100px;
    left:200px;
}
.star6{
    position: absolute;
    top:330px;
    left:230px;
}
.star7{
    position: absolute;
    top:130px;
    left: 500px;
}
.star8{
    position: absolute;
    top:400px;
    left: 550px;
}

@media (min-width:600px) {
    .hero-women{
        width: 500px;
        margin-left: 0;
    }
    
    .hero-container{
        width:90%;
        height: 550px;
    }

    .hero-sub-title{
        font-weight: 400;
        font-size: 32px;
        line-height: 48px;
        letter-spacing: -0.05em;
    }
    .text-block{
        position: absolute;
        width: 300px;
        height: 75px;
        content: '';
        z-index: 1;
        transform: rotate(-2deg);
        left: 3%;
    }
    .text-block2{
        position: absolute;
        width: 375px;
        height: 75px;
        content: '';
        z-index: 1;
        transform: rotate(-2deg);
        left: 3%;
    }
    .text-block3{
        position: absolute;
        width: 300px;
        height: 75px;
        content: '';
        z-index: 1;
        transform: rotate(-2deg);
        left: -3%;
        top:-5px;
    }
    .star1{
        position: absolute;
        left:100px;
        top:7%;
    }
    .star2{
        position: absolute;
        top:40%;
        left:-20px;
    }
    .star3{
        position: absolute;
        top:15%;
        left: 400px;
    }
    .star4{
        position: absolute;
        top:60%;
        left: 450px;
    }
    .star5{
        position: absolute;
        top:100px;
        left:200px;
    }
    .star6{
        position: absolute;
        top:330px;
        left:230px;
    }
    .star7{
        position: absolute;
        top:130px;
        left: 500px;
    }
    .star8{
        position: absolute;
        top:400px;
        left: 550px;
    }
}
</style>