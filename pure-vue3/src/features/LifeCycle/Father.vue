<template>
    <div>
        Father
        <Son />
    </div>
</template>

<script lang="ts" setup>
import Son from './Son.vue'
import { onUnmounted, onMounted, onBeforeMount, onBeforeUnmount, } from 'vue'
onMounted(() => {
    console.log('Father onMounted');
})
onUnmounted(() => {
    console.log('Father onUnmounted');
})
onBeforeMount(() => {
    console.log('Father onBeforeMount');
})
onBeforeUnmount(() => {
    console.log('Father onBeforeUnmount');
})
console.log('Father');
</script>