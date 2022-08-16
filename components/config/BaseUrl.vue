<template>
    <div class="flex items-center justify-center">
        <div class="w-3/4 bg-slate-800 mt-10 rounded-lg p-5">
            <h2 class="text-left text-lg"> Base URL </h2>
            <hr class="border-slate-700 my-2.5" />
            <p class="mt-3">
                Type: string , default: "", values: base path.
            </p>
            <p class="mt-3">
                Использование a baseUrl является обычной практикой в ​​приложениях, использующих загрузчики модулей AMD,
                где модули «разворачиваются» в одну папку во время выполнения. Исходники этих модулей могут находиться в
                разных каталогах, но скрипт сборки соберет их все вместе.
            </p>
            <p class="mt-3">
                Параметр baseUrlсообщает компилятору, где искать модули. Предполагается, что все импортируемые модули с
                не относительными именами относятся к файлу baseUrl.
            </p>
            <p class="mt-3">
                Значение baseUrl определяется как:
            </p>
            <ul
                class="list-disc list-inside text-white-700 bg-slate-600 rounded-xl shadow-lg ring-1 ring-slate-900/5 mt-3 p-4 pl-8">
                <li>
                    значение аргумента командной строки baseUrl (если задан относительный путь, он вычисляется на основе
                    текущего каталога)
                </li>
                <li>
                    значение свойства baseUrl в tsconfig.json (если задан относительный путь, он вычисляется на основе
                    местоположения tsconfig.json)
                </li>
            </ul>
            <p class="mt-3">
                Обратите внимание, что на относительный импорт модулей не влияет установка baseUrl, так как они всегда
                разрешаются относительно их импортируемых файлов.
            </p>
        </div>
    </div>
</template>

<script setup lang='ts'>
import { IHello } from '~~/types/types';

const hello = ref<IHello>({
    text: 'Hello World!'
})

</script>

<style lang=" scss" scoped>
</style>
