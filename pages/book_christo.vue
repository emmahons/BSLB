<template>
    <div class="grid grid-cols-12 gap-10 mt-20">
        <div class="col-start-2 mt-10">
            <BackButton />
        </div>
        <div class="col-start-3 col-span-3 space-y-4 overflow-y-auto max-h-[800px] mt-10">
            <img class="h-auto max-w-full" src="/images/christo_cover.png" alt="">
            <img class="h-auto max-w-full" src="/images/christo_1.JPG" alt="">
            <img class="h-auto max-w-full" src="/images/christo_2.JPG" alt="">
            <img class="h-auto max-w-full" src="/images/christo_3.JPG" alt="">

            <!-- Add more images or content if needed -->
        </div>
        <div class="col-start-7 col-end-11 max-h-20 -z-1 grid mt-10">

            <p class="col-start-1  col-span-2 font-medium text-4xl"> Christo, 5600 cubicmeter Package </p>
            <p class="col-start-1 font-medium italic text-3xl">Christo </p>

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
                <div class="italic mb-4 text-end pr-4">1968</div>
                <div class="italic mb-4 text-end pr-4">(geen nummering)</div>
                <div class="italic mb-4 text-end pr-4">29 x 20,5 cm</div>
                <div class="italic mb-4 text-end pr-4">9782492650116</div>
                <div class="italic mb-4 text-end pr-4">C-COLL 7.071 CHRI</div>
            </div>
            <div class="col-start-1 col-span-2 mt-20"> Artists' book documenting the design, construction and
                presentation of Christo's 5,600 cubic meter balloon sculpture at Documenta 4, 1968. Contents consist of
                reproductions of sketches, architectural plans and photographs of the work in progress. Photographs by
                Klaus Baum and Thomas Cugini. No texts.</div>
        </div>

        <div class="col-start-11 mt-10">
            <favorites />
        </div>

    </div>
</template>

<script setup>
import BackButton from '~/components/backbutton.vue';
</script>