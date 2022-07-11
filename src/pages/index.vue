<script setup lang="ts">
	import { useStore } from '@/store';
	import VitailseLogo from '@/assets/logo.png';
	import Userslogo from '@/assets/users.png';
	useHead({
		title: 'Vitailse | Opinionated vite starter template',
	});

	const store = useStore();
	const { t } = useI18n();
</script>

<template>
	<div class="grid place-items-center min-h-[80vh]">
		<div class="grid max-w-lg text-center place-items-center">
			<img :src="Userslogo" width="300" class="mx-auto" />
			<h1 class="uppercase font-bold text-xl mt-10">Profiles</h1>
			<div class="text-sm text-justify">
				<p> Nama : Ramadhan Nur Khadafi</p>
				<p> Date : Samarinda, 29-10-2005</p>
				<p> Region : Islam</p>	
				<p> Gender : Male</p>	
			</div>

			<div class="max-w-lg text-center mt-10">
				<h1 class="uppercase font-bold text-xl">About</h1>
				<p class="text-sm text-justify">
					Di kelas 6 sd mengenal dunia robotic, dan disaat lulus SMP mulai tertarik dengan dunia programming & sampai sekarang masih mengeksplor, mempelajari dunia teknologi/programming 	
				</p>
			</div>

			<div class="grid max-w-lg text-center place-items-center mt-10">
				<h1 class="uppercase font-bold text-xl">Contact</h1>
				<div class="text-sm text-justify ">
					<p>Phone : 08xxxxxxxxxx</p>
					<p>Email : khadafi1675@gmail.com</p>
					<p>Instagram : khdfiiii_</p>

				</div>
			</div>

			<div class="max-w-lg text-center mt-10">
				<h1 class="uppercase font-bold text-xl">Hobby</h1>
				<div class="text-sm text-justify">
					<p>- Searching informasi tentang teknologi</p>
					<p>- Mendengarkan musik</p>
					<p>- Bermain game</p>
				</div>
			</div>

			<div class="max-w-lg text-center mt-10">
				<h1 class="uppercase font-bold text-xl">Skill</h1>
				<div class="text-sm text-justify">
					<p>- Front end programming skill pemula</p>
					<p>- Back end programming skill pemula</p>
					<p>- Laravel framework (Dalam tahap pembelajaran)</p>
				</div>
			</div>

			<div class="max-w-lg text-center mt-10">
				<h1 class="uppercase font-bold text-xl">Education</h1>
				<div class="text-sm text-justify">
					<p>- Sekolah Dasar : SDN 008 Samarinda</p>
					<p>- Sekolah Menengah : SMPN 21 Samarinda</p>
					<p>- Sekolah Menengah Kejuruan : SMKTI Airlangga Samarinda</p>
				</div>
			</div>

			
			
		</div>
		
	</div>
</template>

<route lang="yaml">
name: home
</route>