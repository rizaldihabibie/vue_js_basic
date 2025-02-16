<script setup>
    console.info('Hello guys')
    const helloHtml = "<h1>Hello VHtml</h1>";
    const dataAttributes = {
        id: "hello",
        class: "hello"
    }
</script>

<template>
    <h1 v-bind="dataAttributes">{{ helloHtml }}</h1>
    <div :class="data.class" v-html="helloHtml"></div>
</template>

<style scoped>
    .hello {
        color: green;
    }
</style>