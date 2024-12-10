<template>
    <div class="border-box">
        <h1 class="title"><slot name="title"></slot></h1>
        <slot></slot>
    </div>
</template>

<style scoped>
    .border-box {
        border: 3px dashed white;
        background-color: transparent;
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .title {
        width: 100px;
        background-color: white;
        position: absolute;
        top: -19px;
        left: 50%;
        transform: translate(-50%);
        font-size: 13px;
        border-radius: 3px;
        padding: 0 3px;
        text-align: center;
    }
</style>