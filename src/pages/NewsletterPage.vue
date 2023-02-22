<template>
    <div class="column items-center justify-center q-gutter-y-md" 
    style="background-color:#E5C643;color:white;height:500px"
    >
        <div class="title1 text-center">
            JOIN SHOPPING COMMUNITY TO 
            <br/>
            GET MONTHLY PROMO
        </div>
        <div class="hero-sub-title">
            Type your email down below and be young wild generation
        </div>
        <div class="q-mt-lg">
            <q-input 
            style="width:400px"
            label="Add your email here" 
            color="black" 
            bg-color="white" 
            outlined 
            v-model="email" 
            >
                <template v-slot:append>
                    <q-btn class="q-my-sm" color="black" label="Send"/>
                </template>
            </q-input>
        </div>
        
    </div>
</template>

<script setup lang="ts">

import { ref } from 'vue';
const email = ref('');

</script>

<style>

</style>