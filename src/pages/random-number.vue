<template>
  <div>
    <div class="border-double border-4 border-gray-600 bg-red-700 max-w-sm mb-10 p-5 rounded-md">
    
  
        <div>
          <input type="number" v-model="message" class="rounded-md mb-5 w-full"/>
        <div>
            <button @click="random" class="border border-black rounded-md bg-gray-700 px-2 py-1 text-white hover:bg-black hover:text-yellow-500 ">
              Generate Rng
            </button>
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
</template>

<script>
export default {
  data() {
    return {
      message: "click in the button for math random number",
      msg: "click in the button for random phrase or word",
    };
  },
  methods: {
    random() {
      this.message = Math.floor(Math.random() * 100 + 1);
    },
    rando() {
      const f = [
        "hello",
        "bye",
        "octuber",
        "offline",
        "online",
        "cat",
        "dog",
        "hi",
        "github",
        "javascript",
        "ruby",
        "csharp",
        "wow",
        "fuck",
        "pineapple",
        "apple",
        "otter",
        "follow",
        "commit",
        "think",
        "beautiful",
        "js",
        "topic",
        "book",
        "info",
        "chat",
        "array",
        "condition",
        "hey",
        "who",
        "asked",
        "why",
        "what",
      ];
      const r = Math.floor(Math.random() * f.length);
      this.msg = f[r];
    },
  },
};
</script>
