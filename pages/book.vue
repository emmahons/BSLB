<template>
    <div class="grid grid-cols-12 gap-10 mt-20">
        <div class="col-start-2">
            <BackButton />
        </div>
        <div class="col-start-3 col-span-3 space-y-4 overflow-y-auto max-h-[700px]">
            <img class="h-auto max-w-full" src="/images/int_cover.png" alt="">
            <img class="h-auto max-w-full" src="/images/int_1.JPG" alt="">
            <img class="h-auto max-w-full" src="/images/int_2.JPG" alt="">
            <img class="h-auto max-w-full" src="/images/int_3.JPG" alt="">
            <img class="h-auto max-w-full" src="/images/int_4.JPG" alt="">
            <!-- Add more images or content if needed -->
        </div>
        <div class="col-start-7 col-end-11 max-h-20 -z-1">

            <p class="font-medium text-2xl"> Interfunktionen 9 </p>
            <p class="font-medium italic text-2xl">Heubach, Friedrich Wolfram </p>

        </div>


        <div class="col-start-7 col-span-1 z-30">
            <p class="rajdhani"> language</p>
            <p class="rajdhani"> Publication date</p>
            <p class="rajdhani"> Pages</p>

        </div>
        <div class="col-start-9 col-span-1 ">
            <p class="italic">German</p>
            <p class="italic">German</p>
        </div>
        <div class="col-start-12">
            <favorites />
        </div>
        <div class="col-start-7 col-span-3">
            <p>Artists' publication; Artists' magazines. </p>
        </div>


        <div class="col-start-7 pt-6">
            <h2> more like this</h2>
        </div>




    </div>
</template>

<script setup>
import BackButton from '~/components/backbutton.vue';
</script>