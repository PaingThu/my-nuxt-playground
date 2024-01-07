<template>
    <div>
        <div class="grid grid-cols-4 gap-5">
            <div v-for="product in products" :key="product.id">
                <nuxt-link :to="`/products/${product.id}`">{{ product.title }}</nuxt-link>
            </div>
        </div>
    </div>
</template>

<script setup>
    const { data: products } = useFetch('https://fakestoreapi.com/products')
</script>

<style lang="scss" scoped>

</style>