<template>
    <div class="flex items-center justify-center">
        <div class="w-3/4 bg-slate-800 mt-10 rounded-lg p-5">
            <h2 class="text-left text-lg"> AlwaysStrict </h2>
            <hr class="border-slate-700 my-2.5" />
            <p class="mt-3">
                Type: boolean, default: зависит от strict.
            </p>
            <p class="mt-3">
                Компилятор будет парсить код в strict mode и добавлять “use strict” в выходные файлы.
            </p>
            <p class="mt-3">
                По умолчанию false, но если включен флаг strict, то true.
            </p>
        </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
</style>