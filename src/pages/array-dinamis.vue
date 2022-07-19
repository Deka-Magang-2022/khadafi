<script setup lang="ts">

	useHead({
		title: 'Array Dinamis',
	});

    const daftarArray = [1,1,2,2,3,3,3,4,4,4,4,5,5,5,6,6,6];
    const arrayUnik = [...new Set(daftarArray)];

    console.log(arrayUnik)


	


</script>

<template>
	<div>

	
<div>
    {{ arrayUnik }}
</div>

	

		<router-link
			:to="{ name: 'home' }"
			class="
				mt-5
				hover:text-gray-200
				dark:hover:text-gray-500
				hover:underline
			"
			>{{ $t('pages.home') }}</router-link
		>
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: array-dinamis
</route>
