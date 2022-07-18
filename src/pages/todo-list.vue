<script setup lang="ts">
	import { useStore } from '@/store';
    const store = useStore();
    let variableInput = '';
		useHead({
			title: 'Todo List',
		});
	store.listTodo = [];
	const simpanData = (value) =>{
		store.listTodo.push(value)
	}
	const hapusData = (value) => {
		store.listTodo.splice( value, 1)
	}

	
</script>

<template>
	<div class="grid min-h-[80vh]">
		
		<div>
            <h1>Halaman Todo List</h1>
            <div class="flex">
                <input v-model="variableInput" class="shadow-xl dark:shadow-blue-900 bg-white border-double border-4  border-sky-500  w-full rounded-md dark:bg-black"  type="text">
                <button @click="simpanData(variableInput)" type="button" class="shadow-xl dark:shadow-blue-900 px-4 py-2 border-double border-4 border-sky-500 bg-blue-800 rounded-md ml-3 text-white">Add</button>
            </div>

			<div class="grid grid-cols-1 gap-5 my-10">
				<div class="shadow-xl dark:shadow-blue-900 border-double border-4 border-red-900 dark:border-sky-500 bg-white dark:bg-black px-4 py-2 rounded-md flex justify-between items-center" v-for="(item, index) in store.listTodo" :key="index">
					{{ item }}
					<button class="border-double border-4 border-red-900  bg-red-500 px-4 py-2 rounded-md text-white" @click="hapusData(index)" type="button">Hapus</button>
				</div>
			</div>

            
        </div>
        
        
			
		

		
        
        
        <router-link
			:to="{ name: 'home' }"
			class="
				mt-5
				hover:text-blue-800
				dark:hover:text-gray-500
				hover:underline
			"
			>{{ $t('pages.home') }}</router-link
		>
		
	</div>
</template>

<route lang="yaml">
name: todo-list
</route>