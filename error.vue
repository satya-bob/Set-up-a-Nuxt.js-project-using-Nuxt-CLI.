<template>
    <div>
        <p>{{ error.statusCode }}</p>
        <p>oops..</p>
        <p>{{ error.message }}</p>

        <button @click="handleError()">go home</button>

    </div>
</template>

<script setup>
defineProps(['error'])

const handleError = () => clearError({ redirect : '/'})

</script>

<style  scoped>

</style>