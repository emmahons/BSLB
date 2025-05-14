<template>
    <div>
        <nav class="header mb-2 bg-white">
            <ul class="flex flex-row justify-end gap-8 mr-12">
                <li class="pr-2">
                    <NuxtLink to="/collections">Collecties</NuxtLink>
                </li>
                <li class="pr-2">
                    <NuxtLink to="/aboutus">Evenementen</NuxtLink>
                </li>
                <li class="pr-2">
                    <NuxtLink to="/aboutus">Praktisch</NuxtLink>
                </li>
                <li class="pr-2">
                    <NuxtLink to="/Search">Search</NuxtLink>
                </li>
            </ul>
        </nav>
    </div>
</template>

<style>
li {
    display: block;
}

.header {
    font-family: 'rajdhani';
    font-size: large;
    font-kerning: 100;
}
</style>
