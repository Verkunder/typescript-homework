<template>
    <div class="flex items-center justify-center">
        <div class="w-3/4 bg-slate-800 mt-10 rounded-lg p-5">
            <h2 class="text-left text-lg"> Что такое псевдонимы путей? </h2>
            <hr class="border-slate-700 my-2.5" />
            <p class="mt-3">
                В TypeScript вы можете избежать этих «плохих» импортов с помощью псевдонимов путей. С псевдонимами пути
                вы можете объявить псевдонимы, которые сопоставляются с определенным абсолютным путем в вашем
                приложении.
            </p>
            <p class="mt-3">
                Пример:
                <code class="text-teal-500">import { User } from '@modules/user/model'; </code>
            </p>
            <p class="mt-3">
                <code class="text-teal-500">@modules</code> сопоставляются с <code
                    class="text-teal-500">'./src/rest/modules'</code>
            </p>
        </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
</style>