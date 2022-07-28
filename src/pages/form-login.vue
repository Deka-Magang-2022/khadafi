<script setup lang="ts">
	useHead({
		title: 'Form Login',
	});
    

	


</script>

<template>
	<div class="-mx-8">

        <div class="-mt-8 max-h-screen  bg-green-300 text-gray-800 antialiased px-4 py-6 flex flex-col justify-center items-center sm:py-12">
            <div class="py-3 text-center">
                <span class="text-2xl font-serif">Login to Shave</span>
                <div class="mt-4 w-96 bg-white shadow-md sm:rounded-lg text-left rounded-t-md">
                    <div class="h-2 bg-green-400 rounded-t-md"></div>
                    <div class="py-6 px-8">
                        <label class="block font-semibold">Username or Email</label>
                        <input type="text" placeholder="Email" class=" border w-full h-5 px-3 py-5 mt-2 hover:outline-none focus:outline-none focus:ring-1 focus:ring-indigo-600 rounded-md">
                        <label class="block mt-3 font-semibold">Password</label>
                        <input type="password" placeholder="Password" class=" border w-full h-5 px-3 py-5 mt-2 hover:outline-none focus:outline-none focus:ring-1 focus:ring-indigo-600 rounded-md">
                        <div class="flex justify-between items-baseline">
                            <button class="mt-4 bg-green-900 hover:bg-green-400 hover:text-black text-white py-2 px-6 rounded-lg">Login</button>
                            <a href="#" class="text-sm hover:underline">Forgot password?</a>
                        </div>
                    </div>
                </div>
                <div class="mt-3">
                    <span class="text-light">Don't have a account?</span>
                    <a href="form-register" class="font-bold hover:underline"> Sign up!</a>
                </div>
            </div>

            
        </div>
        

        <footer class="max-w-lg mx-auto flex justify-center text-black">
				<router-link :to="{ name: 'home' }" class="
				dark:hover:text-gray-500
				hover:underline
			">{{ $t('pages.home') }}</router-link>
				<span class="mx-3">•</span>
				<a href="halaman" class="hover:underline">Halaman</a>
			</footer>

	

		
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: form-login
</route>
