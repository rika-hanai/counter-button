<script setup>
import { useCounterStore } from '~/store/counter'
import Increment from '@/components/atoms/Increment.vue'
import Decrement from '@/components/atoms/Decrement.vue'
import Reset from '@/components/atoms/Reset.vue'

const counter = useCounterStore()

</script>

<template>
    <div class="flex justify-center mt-11 mb-2">
        <Decrement />
        <div class="px-4">
            <p>count: {{ counter.counter }}</p>
            <p>double: {{ counter.double }}</p>
        </div>
        <Increment />
    </div>
    <div>
        <Reset />
    </div>
    <NuxtLink to='/' class="hover:underline underline-offset-2 ease-in duration-500">
        戻る
    </NuxtLink>
</template>