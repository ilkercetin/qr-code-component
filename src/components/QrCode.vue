<template>
    <div class="qr-code-card">
        <img class="qr-image" :src='qrImageLink'>
        <div class="qr-title"> {{ qrTitle }}</div>
        <div class="qr-description"> {{ qrDescription }}</div>
    </div>
</template>

<script setup lang="ts">
    defineProps<{
        qrImageLink: string,
        qrTitle: string,
        qrDescription: string
    }>()
</script>

<style scoped lang="scss">
    .qr-code-card {
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: hsl(0, 0%, 100%);
        padding: 16px;
        border-radius: 25px;
        font-family: Outfit;
        width: 300px;

        .qr-image {
            width: 100%;
            border-radius: 10px;
        }

        .qr-title {
            margin: 16px 0;
            font-size: 24px;
            font-weight: 700;
            color: hsl(218, 44%, 22%);
        }

        .qr-description {
            width: 80%;
            font-size: 15px;
            margin-bottom: 16px;
            color: hsl(220, 15%, 55%);
        }
    }
</style>
