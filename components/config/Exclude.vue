<template>
    <div class="flex items-center justify-center">
        <div class="w-3/4 bg-slate-800 mt-10 rounded-lg p-5">
            <h2 class="text-left text-lg"> Exclude </h2>
            <hr class="border-slate-700 my-2.5" />
            <p class="mt-3">
                Type: string[], default: ["node_modules", "bower_components", "jspm_packages"].
            </p>
            <p class="mt-3">
                Директива служит для того, чтобы исключать некоторые лишние пути или файлы, которые включились
                директивой include. По умолчанию, опция имеет значение путей пакетных менеджеров npm, bower и jspm, так
                как модули в них уже собраны. Помимо этого, TypeScript будет так же игнорировать папку из опции outDir,
                если она указана. Это папка, куда помещаются собранные артефакты сборки. Логично, что их нужно
                исключить. Если добавить свои значения в эту опцию, то необходимо не забыть восстановить умолчания. Так
                как пользовательские значения не объединяются со значениями по умолчанию. Другими словами, необходимо
                вручную указать корень модулей своего пакетного менеджера.
            </p>
            <p class="mt-3">
                <code class="text-teal-500">
                    {
                        "compilerOptions": {},
                        "exclude": [
                            "node_modules",
                            "./src/**/*.spec.ts"
                        ]
                    }
                </code>
            </p>
            <p class="mt-3">
                Опция exclude не может исключить файлы, указанные через files.
            </p>
            <p class="mt-3">
                Опция exclude не может исключить файлы, если они импортируются в других файлах, которые не исключены.
            </p>
        </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
</style>