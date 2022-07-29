<script setup lang="ts">

	import Img1 from '@/assets/img/tv.png';
	import Img2 from '@/assets/img/hp.jpg';
	import Img3 from '@/assets/img/mac.png';
	import Img4 from '@/assets/img/cartoon.png';
	import Img5 from '@/assets/img/plus.png';




	useHead({
		title: 'Halaman Netflix',
	});


	


</script>

<template>
	<div class="-m-8 grid bg-cover h-screen" style="background-image: url('https://assets.nflxext.com/ffe/siteui/vlv3/c2578c37-8569-4f88-b8f1-67a26a9ddcdd/2e83f3ab-d9d1-4f3a-81cb-2bb62aee8b5f/ID-id-20220725-popsignuptwoweeks-perspective_alpha_website_large.jpg')">
		<div class="border-b-[10px] border-b-gray-800 min-h-screen bg-local place-content-center bg-gradient-to-b from-black via-black/50 to-black">

		
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
		<div class="grid gap-2  bg-gray-800">
			<section class="bg-black h-[477px] flex">
				
				<section>
					<h1 class="text-white text-left text-5xl font-bold ml-20 pt-14 pb-10 mt-20">Nikmati di TV-mu.</h1>
					<h2 class="text-white text-left text-2xl font-[arial] ml-20 ">Tonton di Smart TV, Playstation, 
					<br>Xbox,Chromecast, Apple TV, pemutar Blu-ray,dan
					<br> banyak lagi.</h2>
					
				</section>
					<img class="ml-48 w-[400px] h-96 mt-1" :src="Img1">
			
				
				
			</section>

			<section class="bg-black h-[460px] flex">
				<img class="ml-1 w-[500px] h-96 mt-1 mr-20" :src="Img2">
				<section>
					<h1 class="text-white text-left text-5xl font-bold ml-20 pt-14 pb-10 mt-20">Download acara TV
					<br>untuk menontonnya
					<br>secara offline.
					</h1>
					<h2 class="text-white text-left text-2xl font-[arial] ml-20">Simpan favoritmu dengan mudah agar selalu
					<br>ada acara TV dan film yang bisa ditonton.
					</h2>
				</section>
			</section>

			<section class="bg-black h-[535px] flex">
			
				<section>
					<h1 class="text-white text-left text-5xl font-bold ml-20 pt-14 pb-10 mt-32">Tonton di mana pun.</h1>
					<h2 class="text-white text-left text-2xl font-[arial] ml-20">Streaming film dan acara TV tak terbatas di
					<br>ponsel, tablet, laptop, dan TV-mu.
					</h2>
				</section>

				<img class="ml-32 w-[500px] h-96 mt-20 mr-20" :src="Img3">
			
			</section>

			<section class="bg-black h-[525px] flex">

				<img class="ml-10 w-[500px] h-96 mt-20 mr-10" :src="Img4">
				<section>
					<h1 class="text-white text-left text-5xl font-bold ml-20 pt-14 pb-10 mt-32">Buat profil untuk anak.</h1>
					<h2 class="text-white text-left text-2xl font-[arial] ml-20">Kirim anak-anak untuk bertualang bersama
					<br>karakter favorit mereka di dunia yang dibuat
					<br>khusus untuk mereka—gratis dengan
					<br>keanggotaanmu.
					</h2>
				</section>
			
			</section>
			<section class="bg-black h-[970px]">
			
			<h1 class="text-white font-bold text-5xl mt-20 text-center">Tanya Jawab Umum</h1>

			<section class="text-left flex place-content-center">

			<div class="flex flex-col place-items-start mt-16 gap-2 text-white">
				
			<div>
				
				<p class="border-2  bg-[#303030] border-[#303030] w-[750px] h-[70px] p-5 font-[arial] text-2xl">Apa itu Netflix?</p>
				<div class="flex justify-between">
				<img :src="Img5">
					
				</div>
			</div>

			<div>
				
				<p class="border-2  bg-[#303030] border-[#303030] w-[750px] h-[70px] p-5 font-[arial] text-2xl">Berapa biaya berlangganan Netflix?</p>
			</div>

			<div>
				<p class="border-2  bg-[#303030] border-[#303030] w-[750px] h-[70px] p-5 font-[arial] text-2xl">Di mana saya bisa menonton?</p>
				
			</div>

			<div>
				
				<p class="border-2  bg-[#303030] border-[#303030] w-[750px] h-[70px] p-5 font-[arial] text-2xl">Bagaimana cara membatalkannya?</p>
			</div>

			<div>
				<p class="border-2  bg-[#303030] border-[#303030] w-[750px] h-[70px] p-5 font-[arial] text-2xl">Apa yang bisa ditonton di Netflix?</p>
				
			</div>

			<div>
				
				<p class="border-2  bg-[#303030] border-[#303030] w-[750px] h-[70px] p-5 font-[arial] text-2xl">Apakah Netflix sesuai bagi anak-anak?</p>
			</div>
			</div>


			</section>
			
			
			</section>

			<div class="bg-black h-[426px] ">6</div>
		</div>
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: halaman-netflix
</route>
