<template>
    <div>
        <h1 class="text-center text-4xl font-bold mt-10">
            Typescript - конфиг
        </h1>
        <AlwaysStrict />
        <BaseUrl />
        <Target />
        <Alias />
        <Include />
        <Exclude />
        <TypeRoots />

        <div class="flex items-center justify-center mb-5">
            <div class="mt-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
                <div class="rounded-md shadow">
                    <NuxtLink to='/base-types'
                        class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700 md:py-4 md:text-lg md:px-10">
                        Далее
                    </NuxtLink>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang='ts'>
import BaseUrl from "../components/config/BaseUrl.vue";
import AlwaysStrict from "../components/config/AlwaysStrict.vue";
import Target from "../components/config/Target.vue";
import Alias from "../components/config/Alias.vue";
import Include from "../components/config/Include.vue";
import Exclude from "../components/config/Exclude.vue";
import TypeRoots from "../components/config/TypeRoots.vue";
useHead({
    titleTemplate: 'Typescript - конфиг'
})

interface IProps {
    [key: string]: boolean
}

const test = ref<IProps[]>([{"test": true}, {"test2": false}])

type Coordinate = [number, number]

const testx = ref<Coordinate>([100, 3000])

</script>

<style lang="scss" scoped>
</style>