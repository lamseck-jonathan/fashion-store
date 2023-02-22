<template>
    <div  
    :style="isClothe ? 'width:300px;' : 'width:500px'"  
    class="column q-gutter-sm"
    >
        <div>
            <img 
            :style="isClothe ? 'width:300px;' : 'width:500px'" 
            :src="image"/>
        </div> 
        <div class="row items-center justify-between">
            <div class="column q-gutter-sm">
                <div class="text-weight-bold text-subtitle1">
                    {{ props.title }}
                </div> 
                <div>
                    Explore now
                </div>
            </div> 
            <div>
                <q-btn size="lg" flat icon="arrow_forward" />
            </div>
        </div> 
    </div>
</template>

<script setup lang="ts">
const props = defineProps({
    title:{
        type:String,
        required:true
    },
    image:{
        type:String,
        required:true
    },
    isClothe:{
        type:Boolean,
        default:false
    }
})
</script>

<style>

</style>