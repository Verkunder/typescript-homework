<template>
    <div class="flex items-center justify-center">
        <div class="w-3/4 bg-slate-800 mt-10 rounded-lg p-5">
            <h2 class="text-left text-lg"> Псевдонимы типов </h2>
            <hr class="border-slate-700 my-2.5" />
            <p class="mt-3">
                TypeScript позволяет определять псевдонимы типов с помощью ключевого слова type: <code class="text-teal-500">type id = number | string;</code>
            </p>
            <p class="mt-3">
                Здесь для объединения number|string определяется псевдоним id. 
            </p>
            <p class="mt-3">
                Особенно полезны могут псевдонимы, когда мы имеем дело со сложными объектами 
            </p>
            <p class="mt-3">
                <code class="text-teal-500">type Person = {name: string; age: number};</code>
            </p>
            <p class="mt-3">
                В данном случае определяется псевдоним Person для типа {name: string; age: number}, то есть типа, который представляет сложный объект. Затем этот псевдоним применяется для определения переменных и параметров функции 
            </p>
            <p class="mt-3 font-bold">
                Расширение псевдонимов
            </p>
            <p class="mt-3">
                Одни псевдонимы могут заимствовать или расширять код других. Для этого применяется операция &. Например:
            </p>
            <p class="mt-3">
                <code class="text-teal-500">
                    type Person = {name: string; age: number};<br />
                    type Employee = Person & {company: string};
                </code>
            </p>
            <p class="mt-3">
                В данном случае псевдоним Employee расширяет псевдоним Person, добавляя к нему свойство company, которое представляет тип string. То есть фактически мы имеем дело с типом:
            </p>
            <p class="mt-3">
                <code class="text-teal-500">
                    type Employee = {name: string; age: number; company: string};
                </code>
            </p>
        </div>
    </div>
</template>

<script setup lang='ts'>

</script>

<style lang=" scss" scoped>
</style>
