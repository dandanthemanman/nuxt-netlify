<template>
    <div>
        <h1>tester</h1>
    </div>
</template>

<script setup>

// js6 fetch
// fetch('https://jsonplaceholder.typicode.com/todos/1')
//       .then(response => response.json())
//       .then(json => console.log(json))

// nuxt usefetch hook
const { data, isFetching, error, refresh } = await useFetch("https://jsonplaceholder.typicode.com/todos/1")

console.log(data.value.userId)

</script>

<style lang="scss" scoped>

</style>