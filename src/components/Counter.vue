<script setup>
import {ref} from "vue";
let count = ref({
    number: 0,
    name: "test"
});

function increment() {
    count.value.number++;
}
</script>
<template>
    <div>
        <h1 id="count">Counter: {{ count.number }}</h1>
        <button v-on:click="increment">Increment</button>
    </div>
</template>