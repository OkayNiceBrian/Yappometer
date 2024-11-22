<script setup lang="ts">
    import {ref} from "vue";

    const height = ref(0);

    const setHeight = (h: number) =>{
        height.value = h;
    }
</script>


<template>
    <div class="meter-container">
        <div class="meter-bar" style="height: barHeight"></div>
    </div>
</template>


<script lang="ts">
    export default {
        computed: {
            barHeight() {
                return height.value;
            }
        }
    }
</script>

<style scoped>
    .meter-container {
        display: flex;
        height: 80vh;
        width: 50vw;
        background-color: aquamarine;
        box-shadow: 2px 2px 2px 2px rgba(0, 0, 0, 0.4);
    }

    .meter-bar {
        flex: 1;
        background-color: red;
    }
</style>