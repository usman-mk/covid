<template>
    <div class="col-md-3">
        <div class="card bg-light mb-3 shadow">
            <img :src="post.node.thumbnail_src" class="card-img-top" alt="...">

            <div class="card-body">
                <h4 class="card-title">
                    <nuxt-link :to="{ name: 'posts-id', params: { id: post.confirmed }}">
                        <!-- {{ post.node.edge_media_to_caption.edges[0].node.text }} -->
                        <!-- {{ post.node }} -->
                    </nuxt-link>
                </h4>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            index: 0
        }
    },
    props: {
        post: Object
    }
}
</script>
