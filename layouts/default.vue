<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto py-6 px-10 flex justify-between">
                <ul class="flex gap-10">
                    <li>
                        <NuxtLink to="/">
                            Home
                        </NuxtLink>
                    </li>
                    
                    <li>
                        <NuxtLink to="/about">
                            About
                        </NuxtLink>
                    </li>

                    <li>
                        <NuxtLink to="/products">
                            Products
                        </NuxtLink>
                    </li>
                </ul>
            </nav>
        </header>

        <div class="container mx-auto py-6 px-10">
            <slot />
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .router-link-active {
        color: #12b488;
    }
</style>