<template>
	<div class="container">
        <div class="row">
            <Card v-for="post in posts" :key="post.id" :post="post" />
        </div>
	</div>
</template>

<script>
import axios from '@nuxtjs/axios'
import Card from '@/components/Card'

export default {
    components: {
        Card
    },
    data() {
        return {
            posts: []
        }
    },

    async asyncData({ $axios }) {
        let {data} = await $axios.get('https://www.instagram.com/explore/tags/mkinbkk/?__a=1')
        // console.log(data.graphql.hashtag.edge_hashtag_to_media.edges);

        return {posts: data.graphql.hashtag.edge_hashtag_to_media.edges}
    },
    head: {
        title: 'รายการโพสต์'
    }
}
</script>
