<template>
    <div>
        LifeCycle
        <Father v-if="isShow" />
        <button @click="isShow = !isShow">
            {{ isShow ? '隐藏' : '显示' }}
        </button>
    </div>
</template>

<script lang="ts" setup>
import Father from './Father.vue'
import { onUnmounted, onMounted, onBeforeMount, onBeforeUnmount, ref } from 'vue'
console.log('LifeCycle');
let isShow = ref(true)
onMounted(() => {
    console.log('onMounted LifeCycle');
})
onUnmounted(() => {
    console.log('onUnmounted LifeCycle');
})
onBeforeMount(() => {
    console.log('onBeforeMount LifeCycle');
})
onBeforeUnmount(() => {
    console.log('onBeforeUnmount LifeCycle');
})
</script>