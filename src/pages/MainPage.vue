<template>
    <div class="min-window-height">
        <HomePage/>
        <NewArrivalPage/>
        <PaydayPage/>
        <FavoritePage/>
        <DownloadPage/>
        <NewsletterPage/>
    </div>
</template>

<script setup lang="ts">
import FavoritePage from './FavoritePage.vue';
import HomePage from './HomePage.vue';
import NewArrivalPage from './NewArrivalPage.vue';
import PaydayPage from './PaydayPage.vue';
import DownloadPage from './DonwloadPage.vue'
import NewsletterPage from './NewsletterPage.vue';


</script>

<style>
.min-window-height{
    min-height: 100vh;
}
.main-font{
    font-family: 'Poppins';
    font-style: normal;
}
.title1{
    font-weight: 900;
    font-size: 40px;
    line-height: 50px;
    letter-spacing: 0.06em;
}
.hero-text{
    font-weight: 900;
    font-size: 70px;
    line-height: 70px;
}
.bg-yellow-theme{
    background-color: #EBD96B;
}
.min-window-height{
    min-height: 100vh;
}
</style>