<template>
    <div>
        <h1 class="text-lg font-bold">Serviços</h1>
        <NuxtLink to="/servicos/dsenvolvimento-de-sites">Desenvolvimento de sites</NuxtLink>
        <br>
        <NuxtLink to="/servicos/marketing-digital">Marketing Digital</NuxtLink>
        <br>

        <br>
        <br>

        <div v-if="$fetchState.pending">
            Carregando...
        </div>

        <div v-else>
            <pre>
                <div v-for="service in services" :key="service.id">
                    {{ service.title }}
                </div>
            </pre>
        </div>

        <NuxtChild />
    </div>
</template>
  
<script>
export default {
    name: 'IndexPage',

    head() {
        return {
            title: 'Servicos',
            meta: [
                { hid: 'description', name: 'description', content: '' },
            ],
            bodyAttrs: {
                class: 'bg-gray-400'
            }
        }
    },

    data() {
        return {
            services: []
        }
    },

    async fetch() {
        this.services = await this.$axios.$get('')
    },
}
</script>
  