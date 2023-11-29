<template>
    <v-app style="background: #0f0617;">
        <v-app-bar scroll-behavior="elevate" scroll-threshold="20" flat color="#0f0617" height="120" style="position: relative;background: transparent;">
            <v-app-bar-title>
                <div style="padding-left: 30px;">
                    <span class="logoTag">&lt;dev&gt;</span>
                    <span class="logo">ekuuin</span>
                    <span class="logoTag">&lt;dev/&gt;</span>
                </div>
            </v-app-bar-title>
            <v-spacer></v-spacer>
            <Button style="margin-right: 100px;">
                Contáctame
            </Button>
        </v-app-bar>
        <slot></slot>
    </v-app>
</template>
<script setup>
import Button from './Button.vue';

</script>


<style>
.logo {
    font-size: 2rem;
    color: white;
}

.logoTag {
    font-family: 'Open Source Pro', monospace;
    font-size: 1.7rem;
    font-weight: 300;
    color: gray;
    opacity: 0.5;
}


</style>