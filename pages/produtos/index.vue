<template>
    <div>
        <h1 class="text-lg font-bold">Produtos</h1>
        <NuxtLink to="/produtos/produto-a">Produto A</NuxtLink>
        <br>
        <pre>
            <div v-for="product in products" :key="product.id">
                {{ product.title }}
            </div>
        </pre>
        <br>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Totam, necessitatibus! Autem veritatis
            deserunt doloribus alias sequi! Modi rem neque consequuntur odit nobis, porro harum minima omnis,
            mollitia fugiat nulla et?</p>
    </div>
</template>
  
<script>
export default {
    name: 'IndexPage',

    data() {
        return {

        }
    },
    async asyncData({ $axios }) {
        
        const products = await $axios.$get('https://jsonplaceholder.typicode.com/posts')

        return {
            products
        }
    },
}
</script>
  