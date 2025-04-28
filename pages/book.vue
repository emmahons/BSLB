<template>
    <div class="grid grid-cols-12 gap-10">
        <div class="col-start-2">
            <BackButton />
        </div>
        <div class="col-start-3 col-span-3 space-y-4 overflow-y-auto max-h-[500px]">
            <img class="h-auto max-w-full" src="/images/vb2.jpg" alt="">
            <img class="h-auto max-w-full" src="/images/vb2achter.jpg" alt="">
            <!-- Add more images or content if needed -->
        </div>
        <div class="col-start-7 col-span-4 overflow-y-auto max-h-[700px]">
            <div class="h-auto max-w-full"> 
            <h1> D'l'or </h1>
            <h1>Rosanna Puyol Boralevi </h1>

            <p>more information can come here
                "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
                dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip
                ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
                fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
                deserunt mollit anim id est laborum."</p>
                <p>more information can come here
                "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
                dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip
                ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
                fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
                deserunt mollit anim id est laborum."</p>
                <p>more information can come here
                "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
                dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip
                ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
                fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
                deserunt mollit anim id est laborum."</p>

            <div class="col-start-7 pt-6">
                <h2> more like this</h2>
            </div>
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