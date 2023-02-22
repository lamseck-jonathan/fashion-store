<template>
    <q-layout view="hh lpr fff">
  
      <q-header class="bg-white text-black" height-hint="98">
        <q-toolbar class="row q-gutter-x-lg" style="height:75px" >
          <img style="width:220px" src="../assets/logo.png"/>
          <q-space/>
          <q-btn flat label="Catalogue"/>
          <q-btn flat label="Fashion"/>
          <q-btn flat label="Favourite"/>
          <q-btn flat label="Lifestyle"/>
          <q-btn color="black" label="Sign up"/>
        </q-toolbar>
      </q-header>
  
      <q-page-container>
        <router-view />
      </q-page-container>

      <q-footer class="bg-dark text-white q-px-xl">
        <Footer/>
      </q-footer>
      
    </q-layout>
  </template>
  
  <script setup lang="ts">
  import { ref } from 'vue'
  import Footer from '../components/Footer.vue';
  
      const leftDrawerOpen = ref(false)
      const rightDrawerOpen = ref(false)
  
      function toggleLeftDrawer () {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
      function toggleRightDrawer () {
          rightDrawerOpen.value = !rightDrawerOpen.value
      }
  </script>