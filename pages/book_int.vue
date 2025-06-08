<template>
    <div class="grid grid-cols-12 gap-10 mt-20">
        <div class="col-start-2 mt-10">
            <BackButton />
        </div>
        <div class="col-start-3 col-span-3 space-y-4 overflow-y-auto max-h-[700px] mt-10">
            <img class="h-auto max-w-full" src="/images/int_cover.png" alt="">
            <img class="h-auto max-w-full" src="/images/int_1.JPG" alt="">
            <img class="h-auto max-w-full" src="/images/int_2.JPG" alt="">
            <img class="h-auto max-w-full" src="/images/int_3.JPG" alt="">
            <img class="h-auto max-w-full" src="/images/int_4.JPG" alt="">
            <!-- Add more images or content if needed -->
        </div>

        <div class="col-start-7 col-end-11 max-h-20 -z-1 grid">

            <p class="col-start-1  col-span-2 font-medium text-4xl"> Interfunktionen 9 </p>
            <p class="col-start-1 font-medium italic text-3xl">Heubach, Friedrich Wolfram </p>

            <div class="col-start-1 col-span-1 z-30 mt-20">
                <div class="rajdhani mb-4"> Taal</div>
                <div class="rajdhani mb-4"> Publicatiedatum</div>
                <div class="rajdhani mb-4"> Pagina's</div>
                <div class="rajdhani mb-4"> Formaat</div>
                <div class="rajdhani mb-4"> ISBN</div>
                <div class="rajdhani"> Locatie</div>

                <button class="mt-4 bg-black text-white px-4 py-1 rajdhani text-lg">
                    Beschikbaar
                </button>
            </div>
            <div class="col-start-2 col-span-1 mt-20">
                <div class="italic mb-4 text-end pr-4">Duits</div>
                <div class="italic mb-4 text-end pr-4">1970</div>
                <div class="italic mb-4 text-end pr-4">168</div>
                <div class="italic mb-4 text-end pr-4">20,5 x 13 cm</div>
                <div class="italic mb-4 text-end pr-4">9782492650116</div>
                <div class="italic mb-4 text-end pr-4">C-COLL 7.038 HEUB</div>
            </div>
            <div class="col-start-1 col-span-2 mt-20"> Artists' publications; Artists' magazines.</div>
        </div>

        <div class="col-start-11 mt-10">
            <favorites />
        </div>


        <div class="col-start-7 pt-6">
            <h2> meer zoals dit</h2>
        </div>




    </div>
</template>

<script setup>
import BackButton from '~/components/backbutton.vue';
</script>