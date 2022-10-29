<template>
    <div>
        <div class="bg-gray-100">
            <div class="container mx-auto h-10 flex space-x-4 items-center mb-10">
                <NuxtLink :to="{ name: 'a-empresa' }">A empresa</NuxtLink>
                <NuxtLink :to="{ name: 'servicos' }">Serviços</NuxtLink>
                <NuxtLink :to="{ name: 'produtos' }">Produtos</NuxtLink>
            </div>
        </div>
        <div>
            <div class="container mx-auto">
                <Nuxt />
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: '',
}
</script>