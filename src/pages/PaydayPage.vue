<template>
    <div class="bg-payday min-window-height row justify-between q-pt-xl">
        <div class="image-container relative col-12 col-md-6 order-last lt-md items-center justify-center">
            <div class="relative">
                <img class="star9" src="../assets/star.png"/>
            </div>
            <div class="relative">
                <img class="star10" src="../assets/star.png"/>
            </div>
            <div class="relative">
                <img class="star11" src="../assets/star.png"/>
            </div>
            <div class="relative">
                <img class="star12" src="../assets/star.png"/>
            </div>
            <img class="payday-women" style="width:350px" src="../assets/payday-women2.png"/>
        </div>
        <div class="relative col-12 col-md-6 gt-sm items-center justify-center">
            <div class="relative">
                <img class="star9" src="../assets/star.png"/>
            </div>
            <div class="relative">
                <img class="star10" src="../assets/star.png"/>
            </div>
            <div class="relative">
                <img class="star11" src="../assets/star.png"/>
            </div>
            <div class="relative">
                <img class="star12" src="../assets/star.png"/>
            </div>
            <img class="payday-women" style="width:550px" src="../assets/payday-women2.png"/>
        </div>
        <div class="relative col-12 col-md-6 q-pb-xl column items-md-start items-center justify-center">
            <div class="payday-container">
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
    .image-container{
        height: 350px !important;
    }
    .payday-container{
        width:100%;
        display: flex;
        align-items: center;
        justify-items: center;
        flex-direction: column;
    }
    .payday-women{
        position: absolute;
        bottom: 0;
        left: 0;
    }
    .payday-text{
        font-family: 'Poppins';
        font-style: normal;
        font-weight: 500;
        font-size: 18px;
        line-height: 25px;
    }
    .payday-text1{
        font-family: 'Poppins';
        font-style: normal;
        font-weight: 800;
        font-size: 18px;
        line-height: 25px;
    }
    .relative{
        position: relative;
    }
    .star9{
        position: absolute;
        left:19%;
        top:7%;
    }
    .star10{
        position: absolute;
        top:200px;
        left:10%;
    }
    .star11{
        position: absolute;
        top:70px;
        left: 75%;
    }
    .star12{
        position: absolute;
        top:250px;
        left: 72%;
    }
    .star13{
        position: absolute;
        top:100px;
        left:200px;
    }
    .star14{
        position: absolute;
        top:330px;
        left:230px;
    }
    .star15{
        position: absolute;
        top:130px;
        left: 500px;
    }
    .star16{
        position: absolute;
        top:400px;
        left: 550px;
    }
    @media (min-width:600px) {
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
        .payday-women{
            position: absolute;
            bottom: 0;
            left: 100px;
        }
        .payday-container{
            width:500px;
        }
        .star9{
            position: absolute;
            left:48%;
            top:30px;
        }
        .star10{
            position: absolute;
            top:290px;
            left:35%;
        }
        .star11{
            position: absolute;
            top:100px;
            left: 85%;
        }
        .star12{
            position: absolute;
            top:350px;
            left: 90%;
        }
    }
</style>