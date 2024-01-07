<template>
    <div class="card max-w-sm mx-auto mt-7 text-center">
        <p class="mt-7 text-7xl font-bold">{{ error.statusCode }}</p>
        <p class="mt-7 text-6xl">Ooops!</p>
        <p class="mt-7">{{ error.message }}</p>
        <button class="btn mt-7" @click="clearError({redirect: '/'})">Go Home...</button>
    </div>
</template>

<script setup>
    defineProps(["error"])
</script>

<style lang="scss" scoped>

</style>