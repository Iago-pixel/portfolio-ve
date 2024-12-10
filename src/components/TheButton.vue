<template>
    <button class="button"><slot></slot></button>
</template>

<style scoped>
    .button {
        border: 1px dashed black;
        border-radius: 10px;
        height: 25px;
        width: 100px;
        cursor: pointer;
    }
</style>