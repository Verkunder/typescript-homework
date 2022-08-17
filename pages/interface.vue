<template>
    <div>
        <h1 class="text-center text-4xl font-bold mt-10">
            Интерфейсы
        </h1>
        <div class="flex items-center justify-center">
            <div class="w-3/4 bg-slate-800 mt-10 rounded-lg p-5">
                <h2 class="text-left text-lg"> Интерфейсы объектов</h2>
                <hr class="border-slate-700 my-2.5" />
                <p class="mt-3">
                    Интерфейс определяет свойства и методы, которые объект должен реализовать. Другими словами, интерфейс - это определение кастомного типа данных, но без реализации. В данном случае интерфейсы в TS похожи на интерфейсы в языках Java и C#. Интерфейсы определяются с помощью ключевого слова interface. 
                </p>
                <div class="flex items-center justify-center my-10">
                    <image src='https://w6p.ru/ZGYyODd.png' />
                </div>
                <p class="mt-3">
                    При определении интерфейса мы можем задать некоторые свойства как необязательные с помощью знака вопроса. Подобные свойства реализовать необязательно
                </p>
                <div class="flex items-center justify-center my-10">
                    <image src='https://w6p.ru/Y2FlODM.png' />
                </div>
                <p class="mt-3">
                    Также интерфейс может содержать свойства только для чтения, значение которых нельзя изменять. Такие свойства определяются с помощью ключевого слова readonly
                </p>
                <div class="flex items-center justify-center my-10">
                    <image src='https://w6p.ru/NjkwMDR.png' />
                </div>
                <p class="mt-3">
                    Кроме свойств интерфейсы могут определять функции
                </p>
                <div class="flex items-center justify-center my-10">
                    <image src='https://w6p.ru/ZGQ4ZWN.png' />
                </div>
                <p class="mt-3">
                    Опять же объект, который реализует интерфейс, также обязан реализовать определенную в интерфейсе функцию с тем же набором параметров и тем типом выходного результата. В данном случае функция sayWords() в качестве параметра принимает строку и ничего возвращает, выводя на консоль некоторое сообщение
                </p>
                <p class="mt-3">
                    Интерфейсы могут быть реализованы не только объектами, но и классами. Для этого используется ключевое слово implements
                </p>
                <div class="flex items-center justify-center my-10">
                    <image src='https://w6p.ru/NDg3MWN.png' />
                </div>
                <p class="mt-3">
                    Интерфейсы, как и классы, могут наследоваться
                </p>
                <div class="flex items-center justify-center my-10">
                    <image src='https://w6p.ru/ZjM3NTV.png' />
                </div>
            </div>
        </div>
        <div class="flex items-center justify-center mb-5">
            <div class="mt-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
                <div class="rounded-md shadow">
                    <NuxtLink to='/classes'
                        class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700 md:py-4 md:text-lg md:px-10">
                        Назад
                    </NuxtLink>
                </div>
            </div>
            <div class="mt-5 ml-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
                <div class="rounded-md shadow">
                    <NuxtLink to='/'
                        class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700 md:py-4 md:text-lg md:px-10">
                        В начало
                    </NuxtLink>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
useHead( {
    titleTemplate: 'Typescript - Интерфейсы'
} )
</script>

<style scoped>

</style>