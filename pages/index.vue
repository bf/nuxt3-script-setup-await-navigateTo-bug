<template>
	<div>
	<h1>Nuxt3 script setup await navigateTo() bug</h1>
	<ul>
		<li><NuxtLink to="/navigate-fail2">Bug: top-level await navigateTo() is overwritten</NuxtLink></li>
		<li><NuxtLink to="/navigate-fail3">Bug: top-level await navigateTo() is overwritten with {replace:true}</NuxtLink></li>
		<li><NuxtLink to="/navigate-fail4">Bug: top-level await navigateTo() is overwritten with {replace:true,external:true}</NuxtLink></li>
		<li><NuxtLink to="/navigate-fail">Bug: await navigateTo() does not work after useFetch()</NuxtLink></li>
	</ul>
	</div>
</template>
