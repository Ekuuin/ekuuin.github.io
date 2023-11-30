<template>
    <v-footer height="80px" style="background: transparent; padding: 70px 25px 25px 0; z-index: 1004;">
        <v-spacer></v-spacer>
        <span class="text-footer">&#169; Creado por Edwin Valdés. {{ year }}.</span>
    </v-footer>
</template>

<script setup>
const year = new Date().getFullYear();
</script>

<style>
    .text-footer{
        font-family: 'Open Source Pro', monospace;
        font-size: 1rem;
    }

    @media screen and (max-width: 500px) {
        .text-footer{
            font-size: 0.7rem;
        }
        
    }
</style>