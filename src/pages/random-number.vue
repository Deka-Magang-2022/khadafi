<script setup lang="ts">
	useHead({
		title: 'Random Number'
	});

	import { useStore } from '@/store';
	const store = useStore();
	store.input = '0';
	store.min = 1;
	store.max = 100;

	const generateRandom = () => {
		store.input = Math.floor(Math.random() * store.max + store.min);
	}
</script>

<template>
	<div class="min-h-[80vh] dark:text-black">
    <b>Random Number Generator</b>
		<div class="max-w-lg mb-10 border-double border-4 border-sky-400 rounded-md p-5 bg-gray-600 text-white">
			<div class="w-full">
				<input disabled class="w-full border-double border-4 border-blue-800 rounded-md px-4 py-2 text-right text-black" type="text" v-model="store.input">
			</div>
			<div class="w-full grid grid-cols-2 gap-5 mt-5">
				<div>
					<label class="dark:text-white" for="min">Min</label>
					<input id="min" class="w-full rounded-md px-4 py-2 text-right text-black" type="number" v-model="store.min">
				</div>
				<div>
					<label class="dark:text-white" for="max">Max</label>
					<input id="max" class="w-full rounded-md px-4 py-2 text-right text-black" type="number" v-model="store.max">
				</div>
			</div>
			<div class="w-full grid grid-flow-row gap-5 mt-5">
				<button @click="generateRandom()" type="button" class="border border-gray-700 px-2 py-1 bg-green-600 hover:bg-green-400 rounded-md text-black">
					Click for Generate
				</button>
			</div>
		</div>
		<router-link
			:to="{ name: 'home' }"
			class="
				hover:text-gray-500
				dark:hover:text-gray-200
				hover:underline
				dark:text-white
			"
			>{{ $t('pages.home') }}</router-link
		>
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: random-number
</route>