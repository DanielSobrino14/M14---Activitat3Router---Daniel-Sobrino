<script setup>
import productos from '@/assets/productos.json'
import {RouterLink,RouterView} from 'vue-router';
</script>

<template>
    <ul>
        <li v-for="product in productos" :key="product.id">
            <RouterLink :to="'/productDetail/' + product.id + '/' + product.name + '/' + product.description">{{ product.name }}</RouterLink>
        </li>
    </ul>
</template>    