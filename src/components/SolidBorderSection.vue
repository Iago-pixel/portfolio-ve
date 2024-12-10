<template>
    <section class="solid-border">
        <h1 class="title"><slot name=title></slot></h1>
        <slot></slot>
    </section>
</template>

<style scoped>
    .solid-border {
        border: 5px solid white;
        padding: 1.5rem;
        background-color: transparent;
        position: relative;
        margin: 2rem 0;
    }
    .title {
        display: inline;
        background-color: white;
        position: absolute;
        top: -24px;
        left: 50%;
        transform: translate(-50%);
        font-size: 1rem;
        border-radius: 3px;
        padding: 0 3px;
        text-align: center;
    }
</style>