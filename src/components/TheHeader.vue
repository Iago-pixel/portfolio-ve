<template>
    <header class="header"><h1 class="title">Header</h1><TheButton class="the-button">Button</TheButton></header>
</template>

<script>
    import TheButton from './TheButton.vue';

    export default {
            components: {TheButton}
    }
</script>

<style scoped>
    .header {
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
        background-color: white;
        border-radius: 5px;
        height: 27px;
        margin-bottom: 1rem;
    }
    .title {
        font-size: 1rem;
        display: inline;
        margin: 0;
    }
    .the-button {
        position: absolute;
        right: 10px;
    }
</style>