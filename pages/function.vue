<template>
    <div>
        <h1 class="text-center text-4xl font-bold mt-10">
            Функции
        </h1>
        <FunctionDefinition1 />
        <div class="flex items-center justify-center mb-5">
            <div class="mt-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
                <div class="rounded-md shadow">
                    <NuxtLink to='/literal-types'
                        class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700 md:py-4 md:text-lg md:px-10">
                        Назад
                    </NuxtLink>
                </div>
            </div>
            <div class="mt-5 ml-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
                <div class="rounded-md shadow">
                    <NuxtLink to='/classes'
                        class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700 md:py-4 md:text-lg md:px-10">
                        Далее
                    </NuxtLink>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import FunctionDefinition1 from '../components/function/FunctionDefinition.vue';
useHead( {
    titleTemplate: 'Typescript - Функции'
} )
</script>

<style scoped>

</style>