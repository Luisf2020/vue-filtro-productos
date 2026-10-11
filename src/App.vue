<script setup>
import ProductFilter from './components/ProductFilter.vue';

const productos = [
  { id: 1, nombre: 'Teclado', stock: 8 },
  { id: 2, nombre: 'Mouse', stock: 0 },
  { id: 3, nombre: 'Monitor', stock: 3 },
];
</script>

<template>
  <main>
    <h1>Catalogo</h1>
    <ProductFilter :productos="productos" />
  </main>
</template>
