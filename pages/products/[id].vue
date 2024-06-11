<template>
    <div>
        <ProductDetails :product="product" />
    </div>
</template>

<script setup>
    const { id } = useRoute().params // needs to have the same name as the file
    
    const uri = `https://fakestoreapi.com/products/${id}` // fetch the product details
    const { data: product } = await useFetch(uri)

    console.log(product)

    definePageMeta({
        layout: 'products'
    });
</script>

<style scoped>

</style>