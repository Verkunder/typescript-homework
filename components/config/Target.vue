<template>
    <div class="flex items-center justify-center">
        <div class="w-3/4 bg-slate-800 mt-10 rounded-lg p-5">
            <h2 class="text-left text-lg"> Target </h2>
            <hr class="border-slate-700 my-2.5" />
            <p class="mt-3">
                Type: string, default: ES3, влияет на опции lib, module.
            </p>
            <p class="mt-3">
                Версия стандарта ECMAScript, в которую будет скомпилирован код. Здесь большой выбор: ES3, ES5, ES6 (он
                же ES2015), ES2016, ES2017, ES2018, ES2019, ES2020, ESNext. Для backend приложений/пакетов подойдёт ES6,
                если рассчитываете только на современные версии Node.js и ES5, если хотите поддержать более старые
                версии. На данный момент стандарт ES6, с небольшими оговорками, поддерживается 97.29% браузеров. Так что
                для frontend приложений ситуация аналогичная.
            </p>
        </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
</style>