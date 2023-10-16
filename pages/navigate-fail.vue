<template>
	<h1>This should navigate to /a but it navigates to /b</h1>
</template>

<script setup>
const { data: milk, error: errorMilk } = await useFetch("/api/milk")

if (errorMilk.value) {
	throw errorMilk.value
}

if (milk.value && milk.value.length === 0) {
	await navigateTo("/a")
}

const { data: honey, error: errorHoney } = await useFetch("/api/honey")

if (errorHoney.value) {
	throw errorHoney.value
}

if (honey.value && honey.value.length === 0) {
	await navigateTo("/b")
}
</script>