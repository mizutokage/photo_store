<template>
    <div>
        <post-card
            v-for="post in posts"
            v-bind:key="post.id"
            :post=post
        ></post-card>
    </div>
</template>

<script>
import PostCard from '../components/PostCard.vue'

export default {
    components: {
        PostCard,
    },
    data() {
        return {
            posts: [
                {
                    id: 1,
                    name: "mizuto", 
                    age: "25",
                    thumbnail: {
                        url: "https://picsum.photos/800/400?image=80"
                    }
                },
                {
                    id: 2, 
                    name: "nanako", 
                    age: "23",
                    thumbnail: {
                        url: "https://picsum.photos/800/400?image=90"
                    }
                },
                {
                    id: 3, 
                    name: "mizuki", 
                    age: "19",
                    thumbnail: {
                        url: "https://picsum.photos/800/400?image=100"
                    }
                }
            ]
        }
    },
}
</script>