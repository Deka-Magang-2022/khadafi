<script setup lang="ts">
	useHead({
		title: 'Form Register',
	});


	


</script>

<template>
	<div>

        <div class="max-h-screen rounded-md bg-green-300 text-gray-800 antialiased px-4 py-6 flex flex-col justify-center sm:py-12">
            <div class="relative py-3 sm:max-w-xl mx-auto text-center">
                        <span class="text-2xl font-serif">Welcome to Shave</span>
                <div class="relative mt-4 bg-white shadow-md sm:rounded-lg text-left">
                                <div class="h-2 bg-green-400 rounded-t-md"></div>
                    <div class="py-6 px-8">
                        <label class="block font-semibold">Username</label>
                        <input type="text" placeholder="Username" class=" border w-full h-5 px-3 py-5 mt-2 hover:outline-none focus:outline-none focus:ring-1 focus:ring-indigo-600 rounded-md">

                        <label class="block mt-3 font-semibold">Email</label>
                        <input type="text" placeholder="Email" class=" border w-full h-5 px-3 py-5 mt-2 hover:outline-none focus:outline-none focus:ring-1 focus:ring-indigo-600 rounded-md">

                        <label class="block mt-3 font-semibold">Password</label>
                        <input type="password" placeholder="Password" class=" border w-full h-5 px-3 py-5 mt-2 hover:outline-none focus:outline-none focus:ring-1 focus:ring-indigo-600 rounded-md">

                        <label class="block mt-3 font-semibold">Confirm Password</label>
                        <input type="password" placeholder="Confirm Password" class=" border w-full h-5 px-3 py-5 mt-2 hover:outline-none focus:outline-none focus:ring-1 focus:ring-indigo-600 rounded-md">

                        <div class="flex justify-between items-baseline">
                            <button class="mt-4 bg-green-900 hover:bg-green-400 text-white py-2 px-6 rounded-lg">Confirm</button>
                            <a href="form-login" class="text-sm hover:underline">Back</a>
                        </div>
                    </div>
                </div>
                
            </div>
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
name: form-register
</route>
