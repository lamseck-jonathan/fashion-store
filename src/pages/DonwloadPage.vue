<template>
    <div class="window-height row items-center full-width">
        <div class="col-12 col-md-6 column justify-center items-center">
            <div class="q-gutter-y-md column gt-sm">
                <div style="width:500px" class="main-font title1">
                    DOWNLOAD APP &
                    GET THE VOUCHER!
                </div> 
                <div class="main-font text-subtitle1">
                    Get 30% off for first transaction using <br/>Rondovision mobile app for now.
                </div> 
                <div class="row q-gutter-md">
                    <q-btn no-caps color="black" >
                        <img class="q-mr-sm" style="width:40px" src="../assets/apple_store.png"/>
                        <div class="column">
                            <div class="download-btn-text text-subtitle2 text-weight-regular">
                                Download on the
                            </div>
                            <span class="text-center text-weight-bold text-h6">
                                App Store
                            </span>
                        </div>
                    </q-btn>
                    <q-btn no-caps color="black">
                        <img class="q-mr-sm" style="width:35px" src="../assets/google_play.png"/>
                        <div class="column">
                            <div class="download-btn-text text-subtitle2 text-weight-regular">
                                Get it on
                            </div>
                            <span class="text-center text-weight-bold text-h6">
                                Google Play
                            </span>
                        </div>
                    </q-btn>
                </div> 
            </div>
            <div class="q-gutter-y-md column items-center lt-md q-px-lg">
                <div class="main-font title1 text-center">
                    DOWNLOAD APP &
                    GET THE VOUCHER!
                </div> 
                <div class="main-font text-subtitle1">
                    Get 30% off for first transaction using <br/>Rondovision mobile app for now.
                </div> 
                <div class="row q-gutter-sm">
                    <q-btn no-caps color="black" >
                        <img class="q-mr-sm" style="width:30px" src="../assets/apple_store.png"/>
                        <div class="column">
                            <div class="download-btn-text text-subtitle2 text-weight-regular">
                                Donwload on
                            </div>
                            <span class="text-center text-weight-bold text-subtitle2">
                                App Store
                            </span>
                        </div>
                    </q-btn>
                    <q-btn no-caps color="black">
                        <img class="q-mr-sm" style="width:30px" src="../assets/google_play.png"/>
                        <div class="column">
                            <div class="download-btn-text text-subtitle2 text-weight-regular">
                                Get it on
                            </div>
                            <span class="text-center text-weight-bold text-subtitle2">
                                Google Play
                            </span>
                        </div>
                    </q-btn>
                </div> 
            </div>
        </div>
        <div class="col-12 col-md-6 row justify-center">
            <img class="download-logo" style="" src="../assets/voucher.png"/>
        </div> 
    </div>
</template>

<script setup lang="ts">

</script>

<style>
.download-btn-text{
    text-align: start;
}
.download-logo{
    width:300px
}
@media (min-width:600px) {
    .download-logo{
        width:400px
    }
}
</style>