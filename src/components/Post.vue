<script>
export default {
    name: 'Post',
    data() {
        return {
            grid: [],
            startingNode: -1,
            destinationNode: -1,
            action: -1,
            mousedown: false,
            showError: false
        }
    },
    methods: {

    },
    mounted() {

    }
}
</script>
<template>
    <div class="TypingBox">
        <div class="mx-auto w-80 lg:w-[36rem] text-white rounded-tr-lg rounded-bl-lg min-h-[16rem] font-light bg-gradient-to-br from-slate-800 to-slate-900 overflow-hidden">
            <div class="bg-gradient-to-br from-sky-600 to-blue-700 py-3 px-2 min-h-[3.875rem] flex">

                <div>
                    <div class="rounded-full bg-white p-1 w-fit min-w-[2.375rem] min-h-[2.375rem] ml-3 drop-shadow-xl">
                        <img src="https://picsum.photos/30" alt="" class="rounded-full">
                    </div>
                </div>

                <div class="my-auto font-semibold px-1 ml-3">
                    Mori Calliope
                </div>

            </div>

            <div class="p-6 mb-3 font-sans">
                <p class="mb-5">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur autem cumque in ipsam totam! Accusantium autem doloremque ducimus magni quibusdam?</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ab asperiores atque consectetur et rerum sit.</p>
            </div>

        </div>
    </div>
</template>

<style>
.hide {
    display: none;
}
</style>