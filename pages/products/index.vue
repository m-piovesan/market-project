<template>
    <div class="grid grid-cols-4 gap-5">
        <div v-for="p in products" :key="p.id" class="">
            <ProductCard :product="p" />
        </div>
    </div>
</template>

<script setup>
    definePageMeta({
        title: 'Products',
        description: 'This is the products page',
        layout: 'products'
    });

    const { data: products } = await useFetch('https://fakestoreapi.com/products');
</script>

<style scoped>
    
</style>