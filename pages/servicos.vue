<template>
    <div>
        <div class="bg-gray-100">
            <div class="container mx-auto h-10 flex space-x-4 items-center mb-10">
                <NuxtLink :to="{ name: 'a-empresa' }">A empresa</NuxtLink>
                <NuxtLink :to="{ name: 'servicos' }">Serviços</NuxtLink>
            </div>
        </div>
        <div>
            <div class="container mx-auto">
                <h1 class="text-lg font-bold">Serviços</h1>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Totam, necessitatibus! Autem veritatis
                    deserunt doloribus alias sequi! Modi rem neque consequuntur odit nobis, porro harum minima omnis,
                    mollitia fugiat nulla et?</p>
            </div>
        </div>
    </div>
</template>
  
<script>
export default {
    name: 'IndexPage'
}
</script>
  