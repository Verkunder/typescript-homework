<template>
    <div class="flex items-center justify-center">
        <div class="w-3/4 bg-slate-800 mt-10 rounded-lg p-5">
            <h2 class="text-left text-lg"> Include </h2>
            <hr class="border-slate-700 my-2.5" />
            <p class="mt-3">
                Type string[], default: зависит от значения files , связана с exclude.
            </p>
            <p class="mt-3">
                Если опция files не указана, то TypeScript будет использовать эту директиву для поиска компилируемых
                файлов. Если include так же не указана, то её значение будет неявно объявлено как ["**/*"]. Это
                означает, что поиск файлов будет осуществляться во всех папках и их подпапках. Такое поведение не
                оптимально, поэтому в целях производительности лучше всегда указывать конкретные пути. Можно прописывать
                как пути к конкретным файлам, так и паттерны путей.
            </p>
            <p class="mt-3">
                <code class="text-teal-500">
                    {
                        "compilerOptions": {},
                        "include": [
                            "src/**/*",
                            "tests/**/*"
                        ]
                    }
                </code>
            </p>
            <p class="mt-3">
                Если паттерны не указывают конкретных расширений, то TypeScript будет искать файлы с расширениями .ts,
                .tsx и .d.ts. А если включен флаг allowJs, то ещё .js и .jsx.
            </p>
            <p class="mt-3">
                Следующие форматы записей делают одно и тоже src, ./src, src/**/*. Я предпочитаю вариант ./src.
            </p>
            <p class="mt-3">
                Технически, используя опции include и exclude, TypeScript сгенерирует список всех подходящих файлов и
                поместит их в files. Это можно наблюдать если выполнить команду tsc --showConfig.
            </p>
        </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
</style>