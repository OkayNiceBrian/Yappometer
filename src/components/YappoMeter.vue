<template>
    <div class="meter-container">
        <div class="meter-bar"></div>
    </div>
</template>

<style scoped>
    .meter-container {
        display: flex;
        height: 80vh;
        width: 50vw;
        background-color: aquamarine;
        border: 1px gray solid;
        box-shadow: 2px 2px 2px 2px rgba(0, 0, 0, 0.4);
    }

    .meter-bar {
        flex: 1;
        background-color: red;
    }
</style>