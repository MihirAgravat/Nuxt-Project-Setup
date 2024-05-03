<script setup lang="ts">
import { userStore } from '@/store/user'

const user = userStore()

</script>

<template>
    <div class="h-full flex flex-col items-center justify-center">
        <div class="text-3xl drop-shadow-lg font-black text-blue-500">
            Welcome
        </div>
        <button class="py-2 rounded-lg mt-8 text-white shadow-xl transition-all duration-500 translate-y-1 hover:translate-y-0 hover:shadow-gray-400 font-bold px-3 bg-gray-800" @click="user.increment">
            Count {{ user.count }}
        </button>
    </div>
</template>