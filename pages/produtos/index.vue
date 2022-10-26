<template>
    <div>
        <div>
            <h1 class="text-lg font-bold">Produtos</h1>
            <NuxtLink to="/produtos/produto-a">Produto A</NuxtLink>
            <NuxtLink to="/produtos/produto-b">Produto B</NuxtLink>
            <br>
            <br>

            <div 
            v-for="product in products" :key="product.id"
            class="border-b boder-gray-400 py-3"
            >
                {{ product.title }}
            </div>

            <p>Mussum Ipsum, cacilds vidis litro abertis. Viva Forevis aptent taciti sociosqu ad litora torquent.Copo furadis é disculpa de bebadis, 
                arcu quam euismod magna.Quem num gosta di mim que vai caçá sua turmis!Mais vale um bebadis conhecidiss, que um alcoolatra anonimis.
            </p> 
        </div>
    </div>
    
</template>

<script>
    export default {
        name: '',

        data() {
            return {

            };
        },

        async asyncData({ $axios }) {
            
            const products = await $axios.$get('https://jsonplaceholder.typicode.com/posts?_limit=3')

            return {
                products,
            }
        },

        methods: {},
    };
</script>