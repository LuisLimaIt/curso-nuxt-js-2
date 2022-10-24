<template>
    <div>
        <div class="bg-gray-100">
            <div class="container mx-auto flex items-center space-x-4 h-10 mb-10">
                <NuxtLink :to="{ name: 'a-empresa' }">A empresa</NuxtLink>
                <NuxtLink to="/servicos">Serviços</NuxtLink>
            </div>
        </div>

        <div>
            <div class="container mx-auto">
                <h1 class="text-lg font-bold">A empresa</h1>
                <p>Mussum Ipsum, cacilds vidis litro abertis. Viva Forevis aptent taciti sociosqu ad litora torquent.Copo furadis é disculpa de bebadis, arcu quam euismod magna.Quem num gosta di mim que vai caçá sua turmis!Mais vale um bebadis conhecidiss, que um alcoolatra anonimis.</p>
            </div>
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

        methods: {},
    };
</script>