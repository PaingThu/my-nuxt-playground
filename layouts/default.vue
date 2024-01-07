<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between items-center">
                <nuxt-link to="/" class="brand font-bold">Nuxt Playground</nuxt-link>
                <ul class="flex gap-4">
                    <li><nuxt-link to="/">Home</nuxt-link></li>
                    <li><nuxt-link to="/about">About</nuxt-link></li>
                    <li><nuxt-link to="/products">Products</nuxt-link></li>
                    <li><nuxt-link to="/products/abc">ProductsAbc</nuxt-link></li>
                    <li><nuxt-link to="/login">Logout</nuxt-link></li>
                    <li><nuxt-link to="/nopage">NoPage</nuxt-link></li>
                </ul>
            </nav>
        </header>
        <!-- Page Content -->
        <div class="container mx-auto p-4">
            <slot/>
        </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
    nav{
        .brand{
            color: #00dc82;
            font-size: 1.5rem;
        }
        ul{
            li{
                .router-link-active{
                    color: #00dc82;
                }
            }
        }
    }
</style>