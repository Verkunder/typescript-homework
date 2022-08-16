<template>
    <div>
        <h1 class="text-center text-4xl font-bold mt-10">
            Typescript - основы
        </h1>
        <AlwaysStrict />
        <BaseUrl />
        <Target />
        <Alias />
        <Include />
        <Exclude />
        <TypeRoots />
    </div>
</template>

<script setup>
import BaseUrl from "../components/config/BaseUrl.vue";
import AlwaysStrict from "../components/config/AlwaysStrict.vue";
import Target from "../components/config/Target.vue";
import Alias from "../components/config/Alias.vue";
import Include from "../components/config/Include.vue";
import Exclude from "../components/config/Exclude.vue";
import TypeRoots from "../components/config/TypeRoots.vue";
useHead( {
    titleTemplate: 'Typescript - основы'
} )

</script>

<style lang="scss" scoped>
</style>