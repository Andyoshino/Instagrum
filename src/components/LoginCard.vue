<script>
export default {
    name: 'LoginCard',
    props: ['content'],
    data() {
        return {
        }
    },
    methods: {},
    mounted() {
    }
}
</script>
<template>
    <div class="Post">
        <div
            class="p-3 mx-auto w-80 lg:w-[36rem] text-white rounded-tr-lg rounded-bl-lg h-[22rem] font-light bg-gradient-to-br from-red-500 to-pink-500 overflow-hidden flex flex-wrap content-start gap-6">

            <div class="w-full text-center font-mono font-semibold mt-[4rem]">
                <div class="bg-white text-white w-fit mx-auto text-black py-1 px-2">
                    <span class="underline decoration-sky-600 text-pink-500">Insta</span>
                    <span class="underline decoration-pink-600 text-sky-500">grum</span>
                </div>
            </div>

            <div class="m-auto flex flex-wrap gap-3">
                <div class="flex w-full justify-center">
                    <div class="basis-1/4">
                        uname
                    </div>

                    <div class="">
                        <input type="text" class="rounded-md text-black px-2 focus:outline-none">
                    </div>
                </div>

                <div class="flex w-full justify-center">
                    <div class="basis-1/4">
                        password
                    </div>

                    <div class="">
                        <input type="text" class="rounded-md text-black px-2 focus:outline-none">
                    </div>
                </div>
            </div>

            <div class="w-full">
                <div class="mx-auto w-fit mb-2">
                    <button class="w-[17rem] bg-white text-blue-500 py-1 px-2 font-semibold rounded-md">
                        Register
                    </button>
                </div>

                <div class="mx-auto w-fit">
                    <button class="w-[17rem] bg-white text-pink-500 py-1 px-2 font-semibold rounded-md">
                        Login
                    </button>
                </div>
            </div>

        </div>
    </div>
</template>

<style>
</style>