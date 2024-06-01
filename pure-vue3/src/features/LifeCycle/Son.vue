<template>
    <div>
        Son
    </div>
</template>

<script lang="ts" setup>
import { onUnmounted, onMounted, onBeforeMount, onBeforeUnmount } from 'vue'
console.log('Son');
onMounted(()=>{
    console.log('Son onMounted');
})

onUnmounted(()=>{
    console.log('Son onUnmounted');
})
onBeforeMount(()=>{
    console.log('Son onBeforeMount');
})
onBeforeUnmount(()=>{
    console.log('Son onBeforeUnmount');
})
</script>