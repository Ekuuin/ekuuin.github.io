<template>
    <v-container fluid style="padding: 100px 100px 0 100px;">
        <slot></slot>
    </v-container>
</template>

<script setup>

</script>

<style>
.v-container{
    z-index: 4;
    position: relative;
}

@media screen and (max-width: 1400px) {
    .v-container{
        padding: 16px !important;
    }
}
</style>