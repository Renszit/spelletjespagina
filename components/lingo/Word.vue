<template lang="">
	<div class="flex-1 flex bg-red-100">
		<div class="w-1/5 h-full border-black border-2">
			<p class="text-3xl flex justify-center items-center w-full h-full">
				{{ this.letters[0] }}
			</p>
		</div>
		<div class="w-1/5 h-full border-black border-2">
			<p class="text-3xl flex justify-center items-center w-full h-full">
				{{ this.letters[1] }}
			</p>
		</div>
		<div class="w-1/5 h-full border-black border-2">
			<p class="text-3xl flex justify-center items-center w-full h-full">
				{{ this.letters[2] }}
			</p>
		</div>
		<div class="w-1/5 h-full border-black border-2">
			<p class="text-3xl flex justify-center items-center w-full h-full">
				{{ this.letters[3] }}
			</p>
		</div>
		<div class="w-1/5 h-full border-black border-2">
			<p class="text-3xl flex justify-center items-center w-full h-full">
				{{ this.letters[4] }}
			</p>
		</div>
	</div>
</template>

<script>
export default {
  name: "Word",
  props: {
    word: {
      type: String,
      required: true,
    },
  },
  data() {
    return { letters: this.word.split("") };
  },
};
</script>
<style lang=""></style>
