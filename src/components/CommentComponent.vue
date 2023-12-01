<template>
  <div class="comment">
    {{ comment }}
  </div>
</template>

<script>
export default {
    name: 'CommentComponent',
    props: {
        comment: String
    }
}
</script>

<style scoped>
.comment {
  background-color: #f2f2f2;
  padding: 10px;
  margin-bottom: 10px;
}
</style>
