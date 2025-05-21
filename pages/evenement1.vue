<template>
    <div class="grid grid-cols-12 gap-10 mt-20">
        <div class="col-start-2">
            <BackButton />
        </div>
        <div class="col-start-3 col-span-3 space-y-4 overflow-y-auto max-h-[700px]">
            <img class="h-auto max-w-full" src="/images/evenementen/ev1.jpeg" alt="">
            <img class="h-auto max-w-full" src="/images/evenementen/ev1:1.jpeg" alt="">
            <img class="h-auto max-w-full" src="/images/evenementen/ev1:2.jpeg" alt="">
            <!-- Add more images or content if needed -->
        </div>
        <div class="col-start-7 col-span-4 overflow-y-auto max-h-[700px]">
            <div class="h-auto max-w-full">
                <p class="font-medium text-2xl"> Reports from a classroom </p>
                <p class="font-medium italic text-2xl"> Dirk Lauwaert </p>
                <div class="col-start-7 col-span-1">
                    <p class="rajdhani col-span-1"> Book Club</p>
                    <p class="rajdhani"> Wednesday May 28</p>
                    <p class="rajdhani"> 7 PM</p>
                </div>



                <p>Dear readers,
                    The last essay in our triptych on art education after “Poor Artists” and “Let’s talk about Critique”
                    is “Reports from a Classroom” by art critic, writer and former colleague Dirk Lauwaert (1944 -
                    2013). The original Dutch text “Berichten uit een klas” originally appeared in De Witte Raaf 50
                    (July - August 1994). “Berichten uit een klas” was included in the collection “Artikels” (Brussels:
                    Gevaert, 1996).
                    “Reports from a Classroom” - together with 14 other key texts - was published on the occasion of the
                    integration of the Dirk Lauwaert Collection in the Library of Sint-Lukas. Following the writer’s
                    death in 2013, his family loaned his enormous book collection to the school where he taught for many
                    years.
                    As you know we host our monthly Book Club at a special table, designed by Sophie Nys in close
                    colleboration with the librarians, to present books from the Dirk Lauwaert Collection. A most
                    fitting place and text to close the triptych.

                    Lauwaert, D., & Asselberghs, H. (2023). Dirk Lauwaert: Selected Writings, 1983-2008. (R. Desmet, B.
                    Meuleman, & P. J. Perquy, Eds.). Leuven University press. </p>
            </div>
        </div>

        <div class="col-start-12">
            <favorites />
        </div>

    </div>
</template>

<script setup>
import BackButton from '~/components/backbutton.vue';
</script>