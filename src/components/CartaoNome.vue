<script setup>
  defineProps({
    nome: String,
    curso: String
  })  
</script>

<template>
    <section>
         <h2>Lista</h2>

        <p><strong>nome: </strong> {{ nome }}</p>
        <p><strong>Curso: </strong> {{ curso }}</p>
    </section>
</template>

<style scoped>
section{
    background: rgba(7, 61, 0);
    color: white;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 10px 10px 0 rgba(0, 0, 0, 0.3);
    margin: 10px;

}
</style>