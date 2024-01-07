<template>
    <div class="card text-center">
        <img :src="product.image" alt="product thumb" class="thumb">
        <p class="font-bold text-gray-500 m-4 truncate">
            {{ product.title }}
        </p>
        <nuxt-link :to="`/products/${product.id}`" class="btn">
            View Detail
        </nuxt-link>
    </div>
</template>

<script setup>
    const { product } = defineProps(["product"])
</script>

<style lang="scss" scoped>
    .card{
        .thumb{
            max-height: 120px;
            max-width: 70%;
            margin: 0 auto;
        }
    }
</style>