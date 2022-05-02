<template>
    <div class="w-full h-full">
        <p class="mb-10 flex justify-center text-xl font-semibold w-full">
            Lingo Bord {{ this.word }}
        </p>
        <div class="border-2 border-black mx-auto w-4/5 h-3/4 flex flex-col">
            <Word :word="this.word" />
            <Word :word="this.word" />
            <Word :word="this.word" />
            <Word :word="this.word" />
            <Word :word="this.word" />
        </div>

        <div class="mt-10 w-full space-x-3 flex justify-center">
            <form action="">
                <input class="rounded-md" maxLength="5" type="text" />
                <input value="Submit"
                    type="submit"
                    class="border border-black px-3 rounded-md"
                />
            </form>
        </div>
    </div>
</template>

<script>
import Word from './Word.vue'
export default {
    name: 'LingoBoard',
    data() {
        return {
            word: 'lezen',
        }
    },
    components: {
        Word,
    },
}
// 5 rijen
// 5 kolommen
// 5 letters
// 1 rij erbij als het woord niet is geraden
// 1 rij = 1 woord / 1 kans
</script>

<style lang=""></style>
