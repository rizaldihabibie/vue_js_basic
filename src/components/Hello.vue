<script setup>
    console.info('Hello guys')
    const helloHtml = "<h1>Hello VHtml</h1>";
    const classHello = "hello";
    const id = "hello";
    const buttonDisabled = true;
</script>

<template>
    <h1 :id :class ="classHello">{{ helloHtml }}</h1>
    <div v-html="helloHtml"></div>
    <button :disabled="buttonDisabled">This is button</button>
</template>

<style scoped>
    .hello {
        color: green;
    }
</style>