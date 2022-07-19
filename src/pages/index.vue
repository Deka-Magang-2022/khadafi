<script setup lang="ts">
import { useStore } from "@/store";
import VitailseLogo from "@/assets/logo.png";
import Userslogo from "@/assets/user.png";
import Readme from "@/assets/Readme.md";
useHead({
  title: "Vitailse | Opinionated vite starter template",
});

const store = useStore();
const { t } = useI18n();
</script>

<template>
  <div class="grid place-items-center min-h-[80vh]">
    <div class="prose max-w-sm">
      <Readme />
    </div>
    <div
      class="text-yellow-400 dark:text-green-400 outline outline-yellow-400 dark:outline dark:outline-green-300 grid max-w-lg text-center place-items-center bg-black dark:bg-gray-600 rounded-xl py-10 px-5 shadow-2xl shadow-yellow-600 dark:shadow-green-500"
    >
      <img
        :src="Userslogo"
        width="300"
        class="mx-auto rounded-full shadow-xl shadow-yellow-400 dark:shadow-purple-900 outline outline-blue-900 dark:outline-purple-900 bg-cyan-300 dark:bg-purple-400"
      />
      <h1 class="uppercase font-bold text-xl mt-10">Profiles</h1>
      <div class="text-sm text-justify">
        <p>Nama : Ramadhan Nur Khadafi</p>
        <p>Date : Samarinda, 29-10-2005</p>
        <p>Region : Islam</p>
        <p>Gender : Male</p>
      </div>

      <div class="max-w-sm text-center mt-10">
        <h1 class="uppercase font-bold text-xl">About</h1>
        <p class="text-sm text-justify">
          Di kelas 6 sd mengenal dunia robotic, dan disaat lulus SMP mulai tertarik dengan
          dunia programming & sampai sekarang masih mengeksplor, mempelajari dunia
          teknologi/programming
        </p>
      </div>

      <div class="grid max-w-lg text-center place-items-center mt-10">
        <h1 class="uppercase font-bold text-xl">Contact</h1>
        <div class="text-sm text-justify">
          <p>Phone : 08xxxxxxxxxx</p>
          <p>Email : khadafi1675@gmail.com</p>
          <p>Instagram : khdfiiii_</p>
          <a
            href="https://github.com/khdfierror"
            target="_blank"
            class="text-yellow-400 hover:text-white dark:text-green-400 dark:hover:text-sky-200 font-bold"
            >Github</a>
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
          <p>
            <a
              href="https://www.google.co.id/maps/place/Sekolah+Dasar+Negeri+008/@-0.5016369,117.1415925,17z/data=!3m1!4b1!4m5!3m4!1s0x2df67f098bb37527:0x6c6d8d1fe4648b7c!8m2!3d-0.5016423!4d117.1437812"
              target="_blank"
              class="hover:underline"
              >-> Sekolah Dasar : SDN 008 Samarinda</a
            >
          </p>

          <p>
            <a
              href="https://www.google.co.id/maps/place/SMP+Negeri+21+Samarinda/@-0.5072905,117.1558578,17z/data=!3m1!4b1!4m5!3m4!1s0x2df67f9e3a5b4857:0xbe122c6bd7f0845f!8m2!3d-0.5072959!4d117.1580465"
              target="_blank"
              class="hover:underline"
              >-> Sekolah Menengah Pertama : SMPN 21 Samarinda</a
            >
          </p>

          <p>
            <a
              href="https://www.google.co.id/maps/place/SMKTI+Airlangga/@-0.4851169,117.1462529,17z/data=!3m1!4b1!4m5!3m4!1s0x2df67f1489bfeb63:0xe1ef6869246e2125!8m2!3d-0.4851223!4d117.1484416"
              target="_blank"
              class="hover:underline"
              >-> Sekolah Menengah Kejuruan : SMKTI Airlangga Samarinda</a
            >
          </p>
        </div>
      </div>

      <div class="grid grid-flow grid-cols-3 gap-10">
        <a
          href="/todo-list"
          class="bg-blue-900 border-double border-4 border-sky-500 rounded-md mt-5 text-center hover:text-gray-500 dark:hover:text-black hover:underline"
          >Halaman Todo List</a
        >
        <a
          href="/jurnal-harian"
          class="bg-blue-900 border-double border-4 border-sky-500 rounded-md mt-5 text-center hover:text-gray-500 dark:hover:text-black hover:underline"
          >Halaman Jurnal Harian</a
        >
        
        <a
          href="/kalkulator"
          class="bg-blue-900 border-double border-4 border-sky-500 rounded-md mt-5 text-center hover:text-gray-500 dark:hover:text-black hover:underline"
          >Kalkulator</a
        >

        <div class="flex items-center">
          <a href="color-switcher" class="bg-blue-900 border-double border-4 py-2 px-4 border-sky-500 rounded-md mt-5 text-center hover:text-gray-500 dark:hover:text-black hover:underline">
            Color Switcher
          </a>
        </div>
        
        <div class="flex items-center">
          <a href="random-number" class="bg-blue-900 border-double border-4 py-2 px-4 border-sky-500 rounded-md mt-5 text-center hover:text-gray-500 dark:hover:text-black hover:underline">
            Random Number
          </a>
        </div>


      </div>
    </div>
  </div>
</template>

<route lang="yaml">
name: home
</route>
