<script setup lang="ts">
import QrCode from "./components/QrCode.vue";
import imgUrl from './assets/images/image-qr-code.png';
</script>

<template>
    <qr-code :qr-image-link='imgUrl'
             qr-title="Improve your front-end skills by building projects"
             qr-description="Scan the QR code to visit Frontend Mentor and take your coding skill to the next level"/>
</template>

<style>
    body {
        background-color: hsl(212, 45%, 89%);
    }
</style>
