<template>
    <div>
        <nav class="header mb-2">
            <ul class="flex flex-row justify-end gap-8">
                <li class="pr-2">
                    <NuxtLink to="/collections">Collections</NuxtLink>
                </li>
                <li class="pr-2">
                    <NuxtLink to="/aboutus">About</NuxtLink>
                </li>
                <li class="pr-2">
                    <NuxtLink to="/account">Account</NuxtLink>
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
}
</style>
