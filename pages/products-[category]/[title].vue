<script lang="ts" setup>
const route = useRoute();
definePageMeta({
  validate: route => {
    const regex = /^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$/;
    const expresion = new RegExp(regex);
    const title = route.params.title as string;
    return expresion.test(title);
  },
});
</script>

<template>
  <div class="container">
    <h1>Ruta con parametros</h1>
    <h1>parametro 1: {{ route.params.title }}</h1>
    <h1>parametro 2: {{ route.params.category }}</h1>
  </div>
</template>