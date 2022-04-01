<script>
export default {
    name: 'Post',
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
            class="group transition hover:scale-110 mx-auto w-80 lg:w-[36rem] text-white rounded-tr-lg rounded-bl-lg min-h-[11rem] font-light bg-gradient-to-br from-slate-800 to-slate-900 overflow-hidden">
            <div class="group-hover:from-rose-500 group-hover:to-pink-500 bg-gradient-to-br from-sky-600 to-blue-700 py-3 px-2 min-h-[3.875rem] flex">

                <div>
                    <div class="rounded-full bg-white p-1 w-fit min-w-[2.375rem] min-h-[2.375rem] ml-3 drop-shadow-xl">
                        <img src="/public/placeholder_profile.png" alt="" class="rounded-full">
                    </div>
                </div>

                <div class="my-auto font-semibold px-1 ml-3 group-hover:underline group-hover:decoration-white">
                    {{ content.author }}
                </div>

            </div>

            <div class="p-6 mb-3 font-light">
                <p>{{content.text}}</p>
            </div>

        </div>
    </div>
</template>

<style>
</style>