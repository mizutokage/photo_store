<template>
    <div>
        <h2>{{ post.name }}</h2>
        <p>{{ post.age }}</p>
        <a href="">
            <v-img
                class="white--text"
                height="170px"
                width="170px"
                v-bind:src="post.thumbnail.url"
            ></v-img>
        </a>
    </div>
</template>

<script>
export default {
    name: "PostCard",
    props: ["post"]
}
</script>