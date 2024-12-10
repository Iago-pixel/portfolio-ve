<template>
    <li class="card"><slot></slot></li>
</template>

<style scoped>
    .card {
        border-radius: 15px;
        background-color: white;
        display: flex;
        justify-content: center;
        align-items: center;
        font-weight: bold;
        height: 150px;
        width: 290px;
    }
</style>