<template>
    <q-layout view="hhh lpr fff">
  
      <q-header class="bg-white text-black" height-hint="98">
        <q-toolbar class="row q-gutter-x-lg gt-sm" style="height:75px" >
          <img class="main-logo" src="../assets/logo.png"/>
          <q-space/>
          <div class="row q-gutter-x-lg gt-sm">
            <q-btn to="#home" flat label="Home"/>
            <q-btn to="#new_arrival" flat label="Fashion"/>
            <q-btn to="#payday" flat label="Promotion"/>
            <q-btn to="#favorite" flat label="Favourite"/>
            <q-btn to="#download" flat label="Donwload"/>
            <q-btn color="black" label="Sign up"/>
          </div>
          <div class="lt-md">
            <q-btn dense flat round icon="menu" @click="toggleRightDrawer" />
          </div>
        </q-toolbar>
        <q-toolbar class="bg-white text-black full-width fixed row q-gutter-x-lg lt-md" style="height:78px" >
          <img class="main-logo" src="../assets/logo.png"/>
          <q-space/>
          <div class="row q-gutter-x-lg gt-sm">
            <q-btn to="#home" flat label="Home"/>
            <q-btn to="#new_arrival" flat label="Fashion"/>
            <q-btn to="#payday" flat label="Promotion"/>
            <q-btn to="#favorite" flat label="Favourite"/>
            <q-btn to="#download" flat label="Donwload"/>
            <q-btn color="black" label="Sign up"/>
          </div>
          <div class="lt-md">
            <q-btn dense flat round icon="menu" @click="toggleRightDrawer" />
          </div>
        </q-toolbar>
      </q-header>
      <q-drawer v-model="rightDrawerOpen" side="right" bordered>
        <div class="column items-center justify-center q-gutter-md">
          <div class="q-py-lg text-subtitle1">Menu</div>
          <QSeparator color="black"/>
          <q-btn 
              @click="toggleRightDrawer" 
              class="text-center" 
              to="#home" 
              flat 
              label="Home"
          />
          <q-btn 
              @click="toggleRightDrawer" 
              class="text-center" 
              to="#new_arrival" 
              flat 
              label="Fashion"
          />
          <q-btn @click="toggleRightDrawer" 
              class="text-center" 
              to="#payday" 
              flat 
              label="Promotion"
          />
          <q-btn @click="toggleRightDrawer" 
              class="text-center" 
              to="#favorite" 
              flat 
              label="Favourite"
          />
          <q-btn @click="toggleRightDrawer" 
              class="text-center" 
              to="#download" 
              flat 
              label="Donwload"
          />
          <q-btn 
              @click="toggleRightDrawer" 
              class="text-center" 
              color="black" 
              label="Sign up"
          />
        </div>
      </q-drawer>
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

  const rightDrawerOpen = ref(false)
  
  function toggleRightDrawer () {
      rightDrawerOpen.value = !rightDrawerOpen.value
  }
  </script>

<style>
.main-logo{
  width: 200px;
}
@media (min-width: 600px) {
  .main-logo{
    width: 220px;
  }
}
</style>