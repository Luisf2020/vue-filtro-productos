<script setup>
import { computed, ref } from 'vue';

const props = defineProps({
  productos: { type: Array, required: true },
});

const texto = ref('');
const soloDisponibles = ref(false);

const filtrados = computed(() =>
  props.productos.filter((p) => {
    const coincide = p.nombre.toLowerCase().includes(texto.value.toLowerCase());
    return coincide && (!soloDisponibles.value || p.stock > 0);
  }),
);
</script>

<template>
  <section class="filtro">
    <input v-model="texto" placeholder="Buscar producto" aria-label="Buscar producto" />
    <label><input type="checkbox" v-model="soloDisponibles" /> Solo disponibles</label>

    <ul>
      <li v-for="p in filtrados" :key="p.id">
        <strong>{{ p.nombre }}</strong>
        <span>{{ p.stock > 0 ? `${p.stock} en stock` : 'agotado' }}</span>
      </li>
    </ul>
    <p v-if="!filtrados.length">Sin resultados.</p>
  </section>
</template>
