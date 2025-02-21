<script setup>
import {ref} from "vue";
let count = ref(0);

function increment() {
    count.value++;
}
</script>
<template>
    <div>
        <h1 id="count">Counter: {{ count }}</h1>
        <button v-on:click="increment">Increment</button>
    </div>
</template>