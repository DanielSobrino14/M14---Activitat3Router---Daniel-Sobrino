<template>
    <h1>Product Detail</h1>
    <p>{{ $route.params.id }}</p>
    <p>{{ $route.params.name }}</p>
    <p>{{ $route.params.description }}</p>
</template>

<script setup>
import productos from '../assets/productos.json'
import { RouterLink } from 'vue-router';
</script>