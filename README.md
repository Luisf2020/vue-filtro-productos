# vue-filtro-productos

![stack: Vue 3](https://img.shields.io/badge/stack--Vue%203-0d9488?style=flat-square) ![stack: Vite](https://img.shields.io/badge/stack--Vite-0d9488?style=flat-square) ![stack: Composition API](https://img.shields.io/badge/stack--Composition%20API-0d9488?style=flat-square) [![Demo](https://img.shields.io/badge/demo-en%20vivo-22c55e?style=flat-square)](https://luisf2020.github.io/vue-filtro-productos/)
![IA: asistido](https://img.shields.io/badge/IA--asistido-6366f1?style=flat-square)

Catalogo con filtro reactivo en Vue 3 (Composition API + script setup + props/computed).

> **Transparencia sobre IA:** este proyecto se desarrollo con asistencia de inteligencia artificial (generacion de codigo, revision y documentacion). El codigo fue leido, ejecutado y probado manualmente antes de publicarse. No declara clientes, metricas ni resultados que no puedan verificarse.

## Problema que resuelve

Filtrar un catalogo por texto y disponibilidad sin re-renderizar todo el arbol en cada tecla.

## Solucion implementada

Componente con Composition API (ref/computed) y props tipadas; el filtrado es una propiedad derivada reactiva y el vacio tiene estado propio.

### Funcionalidades principales

- Composition API con <script setup>
- Props tipadas y computed
- Filtro combinado por texto y stock
- Estado vacio accesible

## Stack

- Vue 3
- Vite
- Composition API

## Estructura

```
src/components/ProductFilter.vue  # filtro reactivo
src/App.vue                        # datos de ejemplo
src/main.js
```

## Puesta en marcha

```bash
npm install
npm run dev
```

## Complejidad del proyecto

**Nivel: Principiante** — Componente presentacional con estado local; sin integraciones externas.

El nivel describe la complejidad tecnica del proyecto, no el grado de dominio de quien lo escribio.

## Despliegue

Demo en vivo: <https://luisf2020.github.io/vue-filtro-productos/>  
Publicado con GitHub Pages (rama `gh-pages`).

## Autor

**Luis Felipe Zuniga Leon** — Desarrollador de software asistido por IA

- GitHub: <https://github.com/Luisf2020>
- Correo: developerluis2@gmail.com
- WhatsApp: +504 3237 0056

---

_Proyecto de portafolio. El desarrollo se apoyo en herramientas de IA bajo revision tecnica humana._
