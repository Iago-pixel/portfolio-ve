<template>
    <section class="section"><slot></slot></section>
</template>

<style scoped>
    .section {
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
        background-color: white;
        border-radius: 5px;
        height: 150px;
        margin: 2rem 0;
    }
</style>