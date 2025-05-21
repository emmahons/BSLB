<template>
    <div class="grid grid-cols-12 gap-10 mt-20">


        <div class="col-start-2 col-span-10">
            <section class="mt-10">
                <h2 class="title  mb-2 px-4">Nieuwe aanwinsten</h2>
                <div class="w-full overflow-x-auto whitespace-nowrap py-4 px-2 scrollbar-hide">
                    <div class="flex inline-flex space-x-4">
                        <img src="/images/na/na1.jpeg" alt="Nick Mauss" class="w-40 object-cover" />
                        <img src="/images/na/na2.jpeg" alt="Nick Mauss" class="w-40 object-cover" />
                        <img src="/images/na/na3.jpg" alt="Nick Mauss" class="w-40 object-cover" />
                        <img src="/images/na/na4.jpeg" alt="Nick Mauss" class="w-40 object-cover" />
                        <img src="/images/na/na5.jpeg" alt="Nick Mauss" class="w-40 object-cover" />
                        <img src="/images/na/na6.jpg" alt="Nick Mauss" class="w-40 object-cover" />
                        <img src="/images/na/na7.jpg" alt="Nick Mauss" class="w-40 object-cover" />
                        <img src="/images/na/na8.jpg" alt="Nick Mauss" class="w-40 object-cover" />
                        <a
                            href="https://luca.limo.libis.be/discovery/search?query=any,contains,acquisitiondate202503LUKASphysical&tab=ALL_CONTENT&search_scope=ALL_CONTENT_PROFILE&vid=32KUL_LUCAWENK:LUCA&lang=nl&offset=0&pcAvailability=false">
                            <button class="mt-6 bg-black text-white px-2 py-2 max-h-20 rajdhani text-m"> Toon
                                alles</button></a>
                    </div>
                </div>
            </section>
        </div>






        <div class="col-start-1 col-span-8">
            <section class="bg-gray-300 p-8 relative -z-10">
                <h2 class="title text-xl text-white mb-4 ml-20">In de vitrine</h2>
                <div class="flex flex-col md:flex-row gap-6">
                    <img src="/images/foto_jazz.png" alt="Jazz book" class="ml-20 w-40 object-cover" />
                    <div>
                        <h3 class="font-semibold text-xl mt-20">It might as well be spring!</h3>
                        <p class="text-m ">
                            The Sight of Jazz: a selection of books from the library collections and some records from
                            the collection of a librarian.
                        </p>

                        <button class="mt-4 bg-black text-white px-4 py-2 rajdhani text-sm">
                            <NuxtLink to="/book">Lees meer</NuxtLink>
                        </button>
                    </div>
                </div>
            </section>
        </div>
        <div class="col-start-9 top-0 right-0 w-80 h-64 mt-20"><img class="" src="/images/vormen/vorm_oog.png" alt="">
        </div>
        <div class="col-start-3 top-0 left-0 w-56 h-40 mt-20"><img class="" src="/images/vormen/vorm_boek.png" alt="">
        </div>
        <div class="col-start-7 col-span-5 ">
            <section class="bg-[#406791] p-8 relative -z-10">
                <h2 class="title text-xl text-gray-100 mb-4">Op de agenda</h2>
                <div class="flex flex-col md:flex-row gap-6 items-start">
                    <img src="/images/jb_cover.png" alt="Nick Mauss" class="w-40 object-cover" />
                    <div>
                        <h3 class="font-semibold">Library Talk #1: Nick Mauss</h3>
                        <p class="italic text-m mt-2">
                            In conversation with Robbrecht Desmet and Camiel van Winkel
                        </p>
                        <p class="text-sm mt-1">Maandag 4.04.2024 — 20:00</p>
                        <button class="mt-4 bg-black text-white px-4 py-2 rajdhani text-sm">Lees meer</button>
                    </div>
                </div>
            </section>
        </div>
        <div class="col-start-1 col-span-6">
            <section class="bg-[#8F9600] p-8 relative -z-10">
                <h2 class="title text-xl text-white mb-4 ml-20">Hoe zoek ik een boek op?</h2>
                <div class="ml-20">
                    <p class="text-m ">
                        Onze bibliothek maakt gebruik van het UDC systeem om boeken te categoriseren. Ben je op zoek
                        naar een specifiek boek? Kom te weten hoe je deze volgens de UDC-classificatie kan opzoeken!
                    </p>
                    <button class="mt-4 bg-black text-white px-4 py-2 rajdhani text-sm">
                        <NuxtLink to="/book">Lees meer</NuxtLink>
                    </button>

                </div>
            </section>
        </div>

    </div>




</template>