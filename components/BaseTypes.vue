<template>
    <div class="flex items-center justify-center">
        <div class="w-3/4 bg-slate-800 mt-10 rounded-lg p-5">
            <h2 class="text-left text-lg"> Типы данных </h2>
            <hr class="border-slate-700 my-2.5" />
            <ul class="list-disc list-inside text-white-700 rounded-xl ring-1 ring-slate-900/5 mt-3 p-4 pl-8">
                <li>
                    Тип Boolean представляет логическое значение true или false
                    <code class="text-teal-500">let isEnabled: boolean = true;</code>
                </li>
                <li>
                    Тип number представляет числа, причем все числа в TypeScript, как и в JavaScript, являются числами с
                    плавающей точкой. Поэтому с помощью данного типа можно определять как целые числа, так и числа с
                    плавающей точкой:
                    <code class="text-teal-500">
                        <p>let age: number = 36; </p>
                        let height: number = 1.68;
                    </code>
                </li>
                <li>
                    String представляет строки. Как и в JavaScript, в TypeScript строки можно заключать в двойные, либо
                    в одинарные кавычки:
                    <code class="text-teal-500">let lastName = 'Johns';</code> <br>
                    Кроме того, TypeScript поддерживает такую функциональность, как шаблоны строк, то есть мы можем
                    задать шаблон в косых кавычках (`), как если бы мы писали обычную строку, и затем в саму строку
                    можно встраивать разные выражения с помощью синтаксиса ${ expr }, где expr - это выражение.
                    Например:
                </li>
                <li>
                    Для представления очень больших чисел в TypeScript добавлен специальный тип bigint. Этот тип
                    позволяет хранить числа больше чем позволяет тип number.
                    <code class="text-teal-500">let isEnabled: boolean = true;</code>
                    <p>Есть два способа определения объекта этого типа. Первый способ - с помощью функции BigInt():</p>
                    <p><code class="text-teal-500">const num1: bigint = BigInt(100);</code></p>
                    <code class="text-teal-500">const num2: bigint = 100n;</code>
                </li>
                <li>
                    Any описывает данные, тип которых может быть неизвестен на момент написания приложения.
                    <p>
                        <code class="text-teal-500">let someVar: any = "hello"; <br>
                            console.log(someVar); // сейчас someVar - это string<br>
                            someVar = 20; <br>
                            console.log(someVar); // сейчас someVar - это number
                        </code>
                    </p>
                    Так как здесь применяется тип any, то данный код скомпилируется без ошибок, несмотря на смену
                    строкового значения на числовое.
                </li>
                <li>
                    Array: массивы
                </li>
                <li>
                    Enum: перечисления
                </li>
                <li>
                    null и undefined: соответствуют значениям null и undefined в javascript
                </li>
                <li>
                    Never: также представляет отсутствие значения и используется в качестве возвращаемого типа функций,
                    которые генерируют или возвращают ошибку
                </li>
            </ul>
            <h2 class="text-left text-lg"> Symbol </h2>
            <hr class="border-slate-700 my-2.5" />
            <ul class="list-disc list-inside text-white-700 rounded-xl ring-1 ring-slate-900/5 mt-3 p-4 pl-8">
                <li>
                    Тип unique symbol Чтобы разрешить обработку символов как уникальных литералов , доступен специальный
                    тип . unique symbol является подтипом symbol и создается только из вызова Symbol() или Symbol.for()
                    или
                    из явных аннотаций типа. Этот тип разрешен только для const объявлений и readonly staticсвойств, и
                    для ссылки на конкретный уникальный символ вам придется использовать typeof оператор. Каждая ссылка
                    на уникальный символ подразумевает полностью уникальную идентификацию, привязанную к данному
                    объявлению.
                </li>
                <li>
                    Symbol.hasInstance - Метод, который определяет, распознает ли объект конструктора объект как один из
                    экземпляров конструктора. Вызывается семантикой оператора instanceof.
                </li>
                <li>
                    Symbol.isConcatSpreadable - Логическое значение, указывающее, что объект должен быть сведен к
                    элементам массива с помощью Array.prototype.concat.
                </li>
                <li>
                    Symbol.iterator - Метод, который возвращает итератор по умолчанию для объекта. Вызывается семантикой
                    оператора for-of.
                </li>
                <li>
                    Symbol.match - Метод регулярного выражения, который сопоставляет регулярное выражение со строкой.
                    Вызывается по String.prototype.matchметоду.
                </li>
                <li>
                    Symbol.replace - Метод регулярного выражения, который заменяет совпадающие подстроки строки.
                    Вызывается по String.prototype.replaceметоду.
                </li>
                <li>
                    Symbol.search - Метод регулярного выражения, который возвращает индекс в строке, соответствующей
                    регулярному выражению. Вызывается по String.prototype.searchметоду.
                </li>
                <li>
                    Symbol.species - Свойство, оцениваемое функцией, которое является функцией-конструктором,
                    используемым для создания производных объектов.
                </li>
                <li>
                    Symbol.split - Метод регулярного выражения, который разбивает строку по индексам, соответствующим
                    регулярному выражению. Вызывается по String.prototype.splitметоду.
                </li>
                <li>
                    Symbol.toPrimitive - Метод, который преобразует объект в соответствующее примитивное значение.
                    Вызывается ToPrimitiveабстрактной операцией.
                </li>
                <li>
                    Symbol.toStringTag - Строковое значение, используемое при создании строкового описания объекта по
                    умолчанию. Вызывается встроенным методом Object.prototype.toString.
                </li>
                <li>
                    Symbol.unscopables - Объект, собственные имена свойств которого являются именами свойств,
                    исключенными из привязок среды «с» связанных объектов.
                </li>
            </ul>
        </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
</style>