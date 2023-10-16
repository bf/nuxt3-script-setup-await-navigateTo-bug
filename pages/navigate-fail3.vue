<template>
	<h1>This should only navigate to /a</h1>
</template>

<script setup lang="ts">
await navigateTo("/a", { replace: true})

await navigateTo("/b", { replace: true})
</script>