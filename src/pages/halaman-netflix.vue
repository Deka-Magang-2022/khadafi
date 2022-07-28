<script setup lang="ts">
	useHead({
		title: 'Halaman Netflix',
	});


	


</script>

<template>
	<div class="-m-8 grid gap-2 bg-cover h-screen" style="background-image: url('https://assets.nflxext.com/ffe/siteui/vlv3/c2578c37-8569-4f88-b8f1-67a26a9ddcdd/2e83f3ab-d9d1-4f3a-81cb-2bb62aee8b5f/ID-id-20220725-popsignuptwoweeks-perspective_alpha_website_large.jpg')">
		<div class="min-h-screen bg-local place-content-center bg-gradient-to-b from-black via-black/50 to-black">

		
			<nav class="w-full py-4 px-8 flex items-center">
				<div class="font-serif text-5xl text-red-600">Netflix</div>

				<div class="ml-auto flex items-center h-full space-x-3">

					

					<select class="rounded-sm bg-transparent border-1 hover: py-2 border-white text-white">
						<option value="" class="bg-gray-500">Bahasa Indonesia</option>
						<option value="" class="bg-gray-500">English</option>
					</select>


					<a href="#" class="border border-black bg-red-600 text-white font-[arial] rounded-sm px-4 py-2">
					Masuk
					</a>
				</div>


			</nav>

			

			<div class="grid place-content-center h-screen py-10">

				<section class="text-white text-center font-[arial]">
				<h1 class=" text-5xl font-semibold  p-5">Film, acara TV tak terbatas,
				<br> dan lebih banyak lagi.</h1>
				<p class="text-2xl p-5">Tonton di mana pun. Batalkan kapan pun.</p>
				<p class="text-xl p-3">Siap menonton? Masukkan email untuk membuat atau memulai lagi keanggotaanmu.</p>
				</section>

				<section class="flex flex-row place-content-center">
					
					<input type="text" placeholder="Alamat E-mail" class="w-[400px] h-[55px]">	
					<button type="submit" class="bg-red-600 w-[100px] h-[55px] text-white font-[arial]">Mulai ></button>
				</section>

			</div>
			

		</div>
		<div class="grid grid-row-6 gap-2  bg-gray-700">
			<div class="bg-black h-[477px]">
				1.
			</div>
			<div class="bg-black h-[460px]">
				2
			</div>
			<div class="bg-black h-[535px]">3</div>
			<div class="bg-black h-[525px]">4</div>
			<div class="bg-black h-[970px] ">5</div>
			<div class="bg-black h-[426px] ">6</div>
		</div>
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: halaman-netflix
</route>
