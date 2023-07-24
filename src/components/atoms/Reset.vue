<script setup>
import { useCounterStore } from '~/store/counter'

const counter = useCounterStore()
function reset() {
    counter.$reset()
}
</script>

<template>
        <button 
        @click="reset()"
        class="bg-red-500 mb-2 px-4 py-2 text-center tracking-wider inline-block text-white text-xs hover:opacity-75 ease-out duration-300"
        >
        reset
        </button>
</template>