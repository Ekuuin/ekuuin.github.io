<template>
    <v-btn variant="plain" flat rounded style="border-width: 2px; cursor: pointer; border: 2px solid currentColor;">
        <span class="btnText">
            <slot>

            </slot>
        </span>
    </v-btn>
</template>
<script setup>
</script>


<style>
.btnText {
    font-family: 'Open Source Pro', monospace;
    font-weight: 800;
    font-size: 1.1rem;
}
</style>