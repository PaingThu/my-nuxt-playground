<template>
    <div class="login mx-auto py-5">
        <header class="">
            <nav class="container shadow-sm p-4 flex justify-center">
                <h2 class="">Nuxt Playground Login</h2>
            </nav>
        </header>
        <div>
            <slot/>
        </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.login{
    width: 400px;
    header{
        
        nav{
            
            background: #00dc82;
            h2{
                font-size: 1.5rem;
                color: white;
            }
        }
    }
}
    
</style>