<script setup>
    import { ref } from 'vue'
    import CartaoNome from './CartaoNome.vue'
    const nomeNovo = ref('')

    const nomes = ref(["Eduardo", "João Vitor", "Arthur"])

    function adicionar(){
        nomes.value.push(nomeNovo.value)
        nomeNovo.value = ''
    }
</script>

<template>
    <section>
        <h2>Lista de nomes</h2>

        <input type="text" v-model="nomeNovo">
        <button @click="adicionar">Adicionar</button>

        <ul>
            <li v-for="nome in nomes" :key="nome">
                {{ nome }}</li>
        </ul>

        <div class = "lista_cards">
            <CartaoNome
            v-for="nome in nomes"
            :nome="nome"
            curso="Computaria"
            />
        </div>
        
    </section>
</template>

