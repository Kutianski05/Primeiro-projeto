<script setup>
  defineProps({
    nome: String,
    curso: String
  })  
</script>

<template>
    <section>
         <h2>Voto </h2>

        <p><strong>nome: </strong> {{ nome }}</p>
        <p><strong>Curso: </strong> {{ curso }}</p>
    </section>
</template>

<style scoped>
section{
    background: green;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 10px 10px 0 rgba(0, 0, 0, 0.3);
    margin: 10px;

}
</style>