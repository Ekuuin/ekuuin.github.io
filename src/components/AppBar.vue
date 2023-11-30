<template>
    <v-app style="background: #0f0617;">
        <v-app-bar flat color="#0f0617" height="120" style="position:relative; background: transparent; ">
            <v-app-bar-title>
                <div class="logo-wrap">
                    <span class="logoTag">&lt;dev&gt;</span>
                    <span class="logo">ekuuin</span>
                    <span class="logoTag">&lt;dev/&gt;</span>
                </div>
            </v-app-bar-title>
            <Button style="margin-right: 100px;">
                <span class="btn-text">Contáctame</span>
                <img class="btn-icon" src="arrow-down.svg" alt="">
            </Button>
        </v-app-bar>
        <slot></slot>
        <Footer></Footer>
    </v-app>
</template>
<script setup>
import Button from './Button.vue';
import Footer from './Footer.vue';

</script>


<style>
.logo-wrap{
    padding-left: 30px;
}

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

.btn-text {
    font-family: 'Open Source Pro', monospace;
    font-weight: 800;
    font-size: 1.1rem;
}

.btn-icon{
 width: 30px;
 height: 30px;   
}

@media screen and (max-width: 900px) {
    .v-btn{
        margin-right: 16px !important;
    }

    .logo-wrap{
        padding-left: 0px;
    }

    .btn-text{
        display: none;
    }
}


</style>