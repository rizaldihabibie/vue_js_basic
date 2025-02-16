<script setup>
    console.info('Hello guys')
    const helloHtml = "<h1>Hello VHtml</h1>";
</script>

<template>
    <h1 class="hello">{{ helloHtml }}</h1>
    <div v-html="helloHtml"></div>
</template>

<style scoped>
    .hello {
        color: green;
    }
</style>