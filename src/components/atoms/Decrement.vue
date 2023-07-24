<script setup>
import { useCounterStore } from '~/store/counter'
const counter = useCounterStore()
</script>
<template>
<button @click="counter.counter--">
    <font-awesome-icon 
    class="text-white rounded-sm bg-blue-500 mt-2 ml-2 px-2 py-2 hover:opacity-75 ease-out duration-300"
    :icon="['fas', 'minus']" />
</button>
</template>