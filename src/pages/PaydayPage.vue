<template>
    <div class="bg-payday window-height row justify-between">
        <div class="relative col">
            <div class="relative">
                <img class="star5" src="../assets/star.png"/>
            </div>
            <div class="relative">
                <img class="star6" src="../assets/star.png"/>
            </div>
            <div class="relative">
                <img class="star7" src="../assets/star.png"/>
            </div>
            <div class="relative">
                <img class="star8" src="../assets/star.png"/>
            </div>
            <img class="payday-women" style="width:550px" src="../assets/payday-women2.png"/>
        </div>
        <div class="relative col column items-start justify-center">
            <div style="width:500px">
                <div class="relative main-font hero-text">
                    <span class="text-block3 bg-white"></span>
                    <div class="lets-word">
                        PAYDAY 
                    </div>
                </div>
                <div class="main-font hero-text">
                    <div class="lets-word">
                        SALE NOW
                    </div>
                </div>
                <div class="payday-text q-mt-lg">
                    Spend minimal $100 get 30% off <br/>voucher code for your next purchase
                </div>
                <div class="payday-text1 q-mt-lg">
                    1 June - 10 June 2021
                </div>
                <div class="payday-text">
                    *Terms & Conditions apply
                </div>
                <div class="q-mt-lg">
                    <q-btn class="q-px-xl q-py-md" color="black" label="Shop now"/>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">

</script>

<style>
    .bg-payday{
        background: linear-gradient(1.32deg, #E0C340 0.13%, #DFC23E 3.97%, #E1C441 7.2%, #E3C743 10.13%, #E4C542 12.98%, #E6C744 15.99%, #E7C845 19.52%, #E5C643 23.96%, #E6C945 30.43%, #E3C743 36.49%, #E9CA48 42.49%, #EDCE49 49.35%, #F0D44C 55.42%, #F4D84F 61.43%, #F6DA52 65.74%, #F7DB53 72.23%, #F9DD55 77.43%, #F9DF56 83.84%, #FAE157 91.52%, #F9DF56 97.87%);
    }
    .relative{
        position: relative;
    }
    .payday-women{
        position: absolute;
        bottom: 0;
        left: 100px;
    }
    .payday-text{
        font-family: 'Poppins';
        font-style: normal;
        font-weight: 500;
        font-size: 25px;
        line-height: 25px;
    }
    .payday-text1{
        font-family: 'Poppins';
        font-style: normal;
        font-weight: 800;
        font-size: 25px;
        line-height: 25px;
    }
</style>