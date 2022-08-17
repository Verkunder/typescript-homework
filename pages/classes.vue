<template>
    <div>
        <h1 class="text-center text-4xl font-bold mt-10">
            Объектно-ориентированное программирование
        </h1>
        <div class="flex items-center justify-center">
            <div class="w-3/4 bg-slate-800 mt-10 rounded-lg p-5">
                <h2 class="text-left text-lg"> Классы</h2>
                <hr class="border-slate-700 my-2.5" />
                <p class="mt-3">
                    TypeScript реализует объектно-ориентированный подход, в нем есть полноценная поддержка классов.
                    Класс представляет шаблон для создания объектов и инкапсулирует функциональность, которую должен
                    иметь объект. Класс определяет состояние и поведение, которыми обладает объект.
                </p>
                <p class="mt-3">
                    Для определения нового класса применяется ключевое слово class <code
                        class="text-teal-500">class User {}</code>
                </p>
                <p class="mt-3">
                    Для хранения состояния объекта в классе определяются поля
                    <code class="text-teal-500">class User {name: string; age: number;}</code>
                </p>
                <p class="mt-3">
                    Здесь определены два поля - name и age, которые имеют типы string и number соответственно.
                    Фактически поля представляют переменные уровня класса, только для их объявления не применяются var и
                    let. По имени объекта мы можем обращаться к этим полям
                </p>
                <h2 class="text-left text-lg mt-3"> Методы</h2>
                <hr class="border-slate-700 my-2.5" />
                <p class="mt-3">
                    Классы также могут определять поведение - некоторые действия, которые должны выполнять объекты этого
                    класса. Для этого внутри класса определяются функции, которые называются методами.
                </p>
                <p class="mt-3">
                    <code class="text-teal-500">
                        class User { <br />
  
                            name: string; <br />
                            age: number; <br />
                            print(){ <br />
                                console.log(`name: ${this.name}  age: ${this.age}`); <br />
                            } <br />
                            toString(): string{ <br />
                                return `${this.name}: ${this.age}`; <br />
                            }
                        }
                    </code>
                </p>
                <p class="mt-3">
                    В отличие от обычных функций для определения методов не указывается ключевое слово function.
                </p>
                <p class="mt-3">
                    Для обращения внутри методов к полям и другим методам класса применяется ключевое слово this,
                    которое указывает на текущий объект этого класса.
                </p>
                <p class="mt-3">
                    Кроме обычных методов классы имеют специальные функции - конструкторы, которые определяются с
                    помощью ключевого слова constructor. Конструкторы выполняют начальную инициализацию объекта.
                </p>
                <div class="flex items-center justify-center my-10">
                    <image src='https://w6p.ru/ZjZiYWI.png' />
                </div>
                <p class="mt-3">
                    Полям класса в процессе работы программы можно присваивать различные значения, которые соответствуют типу полей. Однако TypeScript также позволяет определять поля для чтения, значения которых нельзя изменить (кроме как в конструкторе). Для определения таких полей применяется ключевое слово readonly:
                </p>
                <div class="flex items-center justify-center my-10">
                    <image src='https://w6p.ru/OThhZjY.png' />
                </div>
                <p class="mt-3">
                    Значение полей для чтения можно установить либо при объявлении, либо в конструкторе
                </p>
            </div>
        </div>
        <div class="flex items-center justify-center mb-5">
            <div class="mt-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
                <div class="rounded-md shadow">
                    <NuxtLink to='/function'
                        class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700 md:py-4 md:text-lg md:px-10">
                        Назад
                    </NuxtLink>
                </div>
            </div>
            <div class="mt-5 ml-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
                <div class="rounded-md shadow">
                    <NuxtLink to='/interface'
                        class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700 md:py-4 md:text-lg md:px-10">
                        Далее
                    </NuxtLink>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>

useHead( {
    titleTemplate: 'Typescript - Классы'
} )
</script>

<style scoped>
</style>