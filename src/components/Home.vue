<script>

import Post from "./Post.vue";
import axios from "axios";

export default {
    name: 'Home',
    components: {
        Post
    },
    data() {
        return {
            listPost: [],
            isLoading: true
        }
    },
    methods: {
        delay(time) {
            return new Promise(resolve => setTimeout(resolve, time));
        },
        async fetchData() {

            this.listPost = [];
            for (let i = 0; i < 5; i++) this.listPost.push('');

            this.isLoading = true;

            axios({
                method: "get",
                url: "https://goquotes-api.herokuapp.com/api/v1/random?count=5"
            })
                .then((res) => {
                    this.listPost = res.data.quotes;
                    this.isLoading = false;
                })
                .catch((err) => console.error(err));
        }
    },
    async mounted() {

        for (let i = 0; i < 5; i++) this.listPost.push('');

        this.fetchData();
    }
}
</script>
<template>
    <div class="post-list">
        <Post class="mb-12" v-bind:class="{'animate-pulse' : isLoading}"
              v-for="(post, index) in listPost" v-bind:key="index"
              :content="post"></Post>

        <div class="text-white">
            <div @click="fetchData" class="hover:scale-125 transition w-fit mx-auto bg-gradient-to-br from-rose-500 to-pink-400 py-2 px-3 rounded-xl">
                more post!
            </div>
        </div>
    </div>
</template>

<style>
</style>