<template>
	<h1>This should only navigate to /a</h1>
</template>

<script setup lang="ts">
await navigateTo("/a")

await navigateTo("/b")
</script>