<template>
    <div class="titel">
        <h3 class="pb-10 pl-10">My account </h3>
    </div>

    <div class="pl-20">
        <div>
            <h2> Log in </h2>
            <div class="mt-10 grid grid-cols-1 gap-x-6 gap-y-8 sm:grid-cols-6">
                <div class="sm:col-span-4">
                    <label for="username" class="input block text-sm/6 font-medium text-gray-900">Username</label>
                    <div class="mt-2">
                        <div
                            class="flex items-center rounded-md bg-white outline-1 -outline-offset-1 outline-gray-300 focus-within:outline-2 focus-within:-outline-offset-2 focus-within:outline-indigo-600">
                            <div class="shrink-0 text-base text-gray-500 select-none sm:text-sm/6"></div>
                            <input type="text" name="username" id="username"
                                class="block min-w-0 grow py-1.5 pr-3 pl-1 text-base text-gray-900 placeholder:text-gray-400 focus:outline-none sm:text-sm/6 bg-gray-200"
                                placeholder="name.lastname@student.luca-arts.be">
                        </div>
                    </div>
                </div>
            </div>
            <div class="mt-10 grid grid-cols-1 gap-x-6 gap-y-8 sm:grid-cols-6">
                <div class="sm:col-span-4">
                    <label for="password" class="input block text-sm/6 font-medium text-gray-900">Password</label>
                    <div class="mt-2">
                        <div
                            class="flex items-center rounded-md bg-white outline-1 -outline-offset-1 outline-gray-300 focus-within:outline-2 focus-within:-outline-offset-2 focus-within:outline-indigo-600">
                            <div class="shrink-0 text-base text-gray-500 select-none sm:text-sm/6"></div>
                            <input type="text" name="password" id="password"
                                class="block min-w-0 grow py-1.5 pr-3 pl-1 text-base text-gray-900 placeholder:text-gray-400 focus:outline-none sm:text-sm/6 bg-gray-200"
                                placeholder="">
                        </div>
                    </div>
                    <button type="button" class="button mt-10">log in</button>
                </div>
            </div>
            <hr>

            <h2> Sign Up</h2>
            <div class="mt-10 grid grid-cols-1 gap-x-6 gap-y-8 sm:grid-cols-6">
                <div class="sm:col-span-4">
                    <label for="email" class="input block text-sm/6 font-medium text-gray-900">Email address</label>
                    <div class="mt-2">
                        <div
                            class="flex items-center rounded-md bg-white outline-1 -outline-offset-1 outline-gray-300 focus-within:outline-2 focus-within:-outline-offset-2 focus-within:outline-indigo-600">
                            <div class="shrink-0 text-base text-gray-500 select-none sm:text-sm/6"></div>
                            <input type="text" name="email" id="email"
                                class="block min-w-0 grow py-1.5 pr-3 pl-1 text-base text-gray-900 placeholder:text-gray-400 focus:outline-none sm:text-sm/6 bg-gray-200"
                                placeholder="name.lastname@student.luca-arts.be">
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="mt-10 grid grid-cols-1 gap-x-6 gap-y-8 sm:grid-cols-6">
            <div class="sm:col-span-4">
                <label for="name" class="input block text-sm/6 font-medium text-gray-900">Name</label>
                <div class="mt-2">
                    <div
                        class="flex items-center rounded-md bg-white outline-1 -outline-offset-1 outline-gray-300 focus-within:outline-2 focus-within:-outline-offset-2 focus-within:outline-indigo-600">
                        <div class="shrink-0 text-base text-gray-500 select-none sm:text-sm/6"></div>
                        <input type="text" name="name" id="name"
                            class="block min-w-0  py-1.5 pr-3 pl-1 text-base text-gray-900 placeholder:text-gray-400 focus:outline-none sm:text-sm/6 bg-gray-200"
                            placeholder="">
                    </div>
                </div>
                <label for="last name" class="input block text-sm/6 font-medium text-gray-900">Last name</label>
                <div class="mt-2">
                    <div
                        class="flex items-center rounded-md bg-white outline-1 -outline-offset-1 outline-gray-300 focus-within:outline-2 focus-within:-outline-offset-2 focus-within:outline-indigo-600">
                        <div class="shrink-0 text-base text-gray-500 select-none sm:text-sm/6"></div>
                        <input type="text" name="last name" id="last name"
                            class="block min-w-0  py-1.5 pr-3 pl-1 text-base text-gray-900 placeholder:text-gray-400 focus:outline-none sm:text-sm/6 bg-gray-200"
                            placeholder="">
                    </div>
                </div>
            </div>
        </div>
        <div class="mt-10 grid grid-cols-1 gap-x-6 gap-y-8 sm:grid-cols-6">
            <div class="sm:col-span-4">
                <label for="password" class="input block text-sm/6 font-medium text-gray-900">Password</label>
                <div class="mt-2">
                    <div
                        class="flex items-center rounded-md bg-white outline-1 -outline-offset-1 outline-gray-300 focus-within:outline-2 focus-within:-outline-offset-2 focus-within:outline-indigo-600">
                        <div class="shrink-0 text-base text-gray-500 select-none sm:text-sm/6"></div>
                        <input type="text" name="password" id="password"
                            class="block min-w-0 grow py-1.5 pr-3 pl-1 text-base text-gray-900 placeholder:text-gray-400 focus:outline-none sm:text-sm/6 bg-gray-200"
                            placeholder="">
                    </div>
                </div>
                <button type="button" class="button mt-10">Sign in</button>
            </div>
        </div>
    </div>
</template>

<style>
.input {
    font-family: 'rajdhani';
    font-size: medium;
}

.button {
    background-color: black;
    border: none;
    color: white;
    font-family: "rajdhani";
    font-size: 20px;
    text-align: center;
    text-decoration: none;
    padding: 10px 25px;
}
</style>
