<template>
  <div class="w-full h-full">
    <p>Lingo Bord {{ this.word }}</p>
    <div class="border-2 border-black w-4/5 h-3/4 flex flex-col">
      <Word />
      <Word />
      <Word />
      <Word />
      <Word />
    </div>
  </div>
</template>

<script>
import Word from "./Word.vue";
export default {
  name: "LingoBoard",
  data() {
    return {
      word: "lezen",
    };
  },
  components: {
    Word,
  },
};
// 5 rijen
// 5 kolommen
// 5 letters
// 1 rij erbij als het woord niet is geraden
// 1 rij = 1 woord / 1 kans
</script>

<style lang=""></style>
