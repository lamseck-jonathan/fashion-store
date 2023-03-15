<template>
    <Transition name="nav">
        <div 
        v-if="menuStore.getMenuState"
        class="menu-mobile m-auto grid grid-cols-1 content-center gap-8 bg-white
        font-medium text-purple-light"
        >
            <img ref="vector1" class="absolute z-10 sm:-right-86 vector-1" src="/images/vector-red.png"/>
            <img ref="vector2" class="absolute z-10 -left-96 -bottom-40 vector-2" src="/images/vector-purple.png"/>
            <nuxt-link @click="menuStore.toggleMenuState" class="text-center" to="#home">{{ $t('Home')}}</nuxt-link>
            <nuxt-link @click="menuStore.toggleMenuState" class="text-center" to="#about">{{ $t('About')}}</nuxt-link>
            <nuxt-link @click="menuStore.toggleMenuState" class="text-center" to="#projet">{{ $t('Projet')}}</nuxt-link>
            <nuxt-link @click="menuStore.toggleMenuState" class="text-center" to="#skill">{{ $t('Skills')}}</nuxt-link>
            <nuxt-link @click="menuStore.toggleMenuState" class="text-center" to="#resume">{{ $t('Resume')}}</nuxt-link>
            <nuxt-link @click="menuStore.toggleMenuState" class="text-center" to="#contact">{{ $t('Contact')}}</nuxt-link>
        </div>
    </Transition> 
</template>

<script setup lang="ts">

</script>

<style>
    .nav-enter-from{
        opacity: 0;
    }
    .nav-enter-to{
        opacity: 1;
    }
    .nav-enter-active{
        transition: all 0.5s ease;
    }
    .nav-leave-from{
        opacity: 1;
       
    }
    .nav-leave-to{
        opacity: 0;
    }
    .nav-leave-active{
        transition: all 0.5s ease;
    }
</style>