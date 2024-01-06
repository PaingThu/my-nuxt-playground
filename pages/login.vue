<template>
    <div class="flex flex-col gap-3 p-4 items-center">
        <input type="text" placeholder="Email">
        <input type="text" placeholder="Password">
        <nuxt-link to="/" class="btn">Login</nuxt-link> 
    </div>
</template>

<script setup>
    definePageMeta({
        layout: 'login'
    })
</script>

<style lang="scss" scoped>

</style>