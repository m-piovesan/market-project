<template>
    <div class="card text-center flex w-full flex-col gap-4">
        <img
            :src="product.image" 
            alt="" 
            class="h-80 "
        />
        <p class="font-bold text-gray-700 m-4 truncate">{{ product.title }}</p>
        <p>R${{ product.price }}</p>
        <NuxtLink 
            class="btn"
            :to="`/products/${product.id}`"
        >More info</NuxtLink>
    </div>
</template>

<script setup>
    const { product }  = defineProps(['product'])
</script>

<style scoped>

</style>