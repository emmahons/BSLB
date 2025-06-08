<template>
    <div>

        <div class="grid grid-cols-12 gap-10 mt-20">
            <div class="col-start-2 col-span-10">
                <p class="title"> Account</p>
            </div>
            <div class="col-start-3 col-span-4">
                <h2> Algemene instellingen</h2>
                Taal <br>
                color mode
            </div>
            <div class="col-start-7 col-span-4">
                <h2> Persoonlijke instellingen</h2>
                Naam <br> Email adress <br> Wachtwoord
            </div>

            <hr class="col-start-2 col-span-10">
            <div class="col-start-3 col-span-10">
                <h2> Mijn boeken</h2>
                <h1> Mijn favorieten</h1>
                <p> Mijn favorieten</p>
                <div class="w-full overflow-x-auto whitespace-nowrap py-4 px-2 scrollbar-hide">
                    <div class="flex inline-flex space-x-4">
                        <img src="/images/na/na1.jpeg" alt="Nick Mauss" class="w-20 object-cover" />
                        <img src="/images/na/na2.jpeg" alt="Nick Mauss" class="w-20 object-cover" />
                        <img src="/images/na/na3.jpg" alt="Nick Mauss" class="w-20 object-cover" />
                        <img src="/images/na/na4.jpeg" alt="Nick Mauss" class="w-20 object-cover" />
                        <img src="/images/na/na5.jpeg" alt="Nick Mauss" class="w-20 object-cover" />
                        <img src="/images/na/na6.jpg" alt="Nick Mauss" class="w-20 object-cover" />
                        <img src="/images/na/na7.jpg" alt="Nick Mauss" class="w-20 object-cover" />
                        <img src="/images/na/na8.jpg" alt="Nick Mauss" class="w-20 object-cover" />
                    </div>
                </div>
            </div>

            <div class="col-start-3 col-span-10">
                <h1> Wil ik nog lezen</h1>
                <p> Boeken die ik nog graag wil lezen!!</p>
                <div class="w-full overflow-x-auto whitespace-nowrap py-4 px-2 scrollbar-hide">
                    <div class="flex inline-flex space-x-4">
                        <img src="/images/co_cover.png" alt="Nick Mauss" class="w-20 object-cover" />
                        <img src="/images/jd_cover.png" alt="Nick Mauss" class="w-20 object-cover" />
                        <img src="/images/JB_cover.png" alt="Nick Mauss" class="w-20 object-cover" />
                        <img src="/images/ngsa_cover.png" alt="Nick Mauss" class="w-20 object-cover" />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>