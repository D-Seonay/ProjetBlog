<template>
  <HeaderComponent />

  <ArticleComponent :article="currentArticle" />

  <FooterComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import FooterComponent from './components/FooterComponent.vue'
import ArticleComponent from './components/ArticleComponent.vue'

export default {
  name: 'ParentComponent',
  components: {
    HeaderComponent,
    FooterComponent,
    ArticleComponent
  },
  data() {
    return {
      currentArticle: {
        title: 'Mon premier article',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed non risus. Suspendisse lectus tortor, dignissim sit amet, adipiscing nec, ultricies sed, dolor.'
      }
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