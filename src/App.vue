<template>
  <HeaderComponent />

  <SidebarComponent />

  <ArticleComponent :article="currentArticle" />

  <CommentComponent :comment="currentCommentaire" />

  <FooterComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import FooterComponent from './components/FooterComponent.vue'
import ArticleComponent from './components/ArticleComponent.vue'
import SidebarComponent from './components/SidebarComponent.vue'
import CommentComponent from './components/CommentComponent.vue'

export default {
  name: 'ParentComponent',
  components: {
    HeaderComponent,
    SidebarComponent,
    FooterComponent,
    ArticleComponent, 
    CommentComponent,
},
  data() {
    return {
      currentArticle: {
        title: 'Mon premier article',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed non risus. Suspendisse lectus tortor, dignissim sit amet, adipiscing nec, ultricies sed, dolor.'
      },
      currentCommentaire: 'Mon premier commentaire'
    }
  }
}
</script>

<style lang="scss">

body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

}
</style>