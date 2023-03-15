<template>
    <div>
        <div class="hamburger z-50" 
        @click="hamburgerClicked" 
        :class="active === true ? 'active' : ''"
        >
            <div class="bar"></div>
            <div class="bar"></div>
            <div class="bar"></div>
        </div>
    </div>  
</template>
    
<script setup lang="ts">import { ref } from 'vue';

    const props = defineProps({
        clicked : {
            type: Boolean,
            default : false
        }
    })
    const active = ref(props.clicked)
    function hamburgerClicked(){

    }
</script>

<style>
    .bar{
        display: block;
        width: 25px;
        height: 3px;
        margin: 5px auto;
        background: black;
        transition: all 0.3s ease-in-out;
    }
    .hamburger{
        cursor: pointer;
        display: block;
    }
    .active .bar:nth-child(2){
        opacity: 0;
    }
    .active .bar:nth-child(1){
        transform: translateY(8px) rotate(135deg);
    }
    .active .bar:nth-child(3){
        transform: translateY(-8px) rotate(45deg);
    }
</style>