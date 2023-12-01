<template>
    <h2>{{ article.title }}</h2>
    <p>{{ article.content }}</p>
    <CommentComponent v-bind:comment="article.comment" />
</template>

<script>
import CommentComponent from './CommentComponent.vue';

export default {
    name: 'ArticleComponent',
    components: {
        CommentComponent
    },
    props: {
        article: Object
    }
}
</script>