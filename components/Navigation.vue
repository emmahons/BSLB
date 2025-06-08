<template>
    <div class=" z-40">
        <nav class="header mb-2 bg-white">
            <ul class="flex flex-row justify-end gap-8 mr-12">
                <li class="pr-2">
                    <NuxtLink to="/collections">Collecties</NuxtLink>
                </li>
                <li class="pr-2">
                    <NuxtLink to="/evenementen">Evenementen</NuxtLink>
                </li>
                <li class="pr-2">
                    <NuxtLink to="/praktisch">Praktisch</NuxtLink>
                </li>
                <li class="pr-2">
                    <NuxtLink to="/account"><svg width="20" height="22" viewBox="0 0 22 24" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M21 22.3333C20.3667 9.88933 1.63333 9.88933 1 22.3333M15 5C15 6.06087 14.5786 7.07828 13.8284 7.82843C13.0783 8.57857 12.0609 9 11 9C9.93913 9 8.92172 8.57857 8.17157 7.82843C7.42143 7.07828 7 6.06087 7 5C7 3.93913 7.42143 2.92172 8.17157 2.17157C8.92172 1.42143 9.93913 1 11 1C12.0609 1 13.0783 1.42143 13.8284 2.17157C14.5786 2.92172 15 3.93913 15 5Z"
                                stroke="black" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
                        </svg></NuxtLink>
                </li>
                <li class="pr-2">
                    <NuxtLink to="/Search"><svg width="20" height="20" viewBox="0 0 24 24" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M18.5239 18.5602L22.6306 22.6668M21.3333 11.3335C21.3333 13.9857 20.2797 16.5292 18.4043 18.4046C16.529 20.2799 13.9854 21.3335 11.3333 21.3335C8.68109 21.3335 6.13755 20.2799 4.26218 18.4046C2.38682 16.5292 1.33325 13.9857 1.33325 11.3335C1.33325 8.68133 2.38682 6.13779 4.26218 4.26243C6.13755 2.38706 8.68109 1.3335 11.3333 1.3335C13.9854 1.3335 16.529 2.38706 18.4043 4.26243C20.2797 6.13779 21.3333 8.68133 21.3333 11.3335Z"
                                stroke="black" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
                        </svg>
                    </NuxtLink>
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
