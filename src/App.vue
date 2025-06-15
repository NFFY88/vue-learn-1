<script setup>
const today = Date.now();
const formattedDate = new Date(today).toLocaleDateString();
</script>

<template>{{ formattedDate }}</template>

<style scoped></style>
