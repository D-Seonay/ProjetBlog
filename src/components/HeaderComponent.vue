<template>

  <header>

      <h1>Mon Blog</h1>
      <nav>
          <!-- Elements nav -->
      </nav>

  </header>

</template>

<script>

  export default {
          name: 'HeaderComponent',
  }

</script>

<style lang="scss">

  @import url('https://fonts.googleapis.com/css?family=Poppins:100,100italic,200,200italic,300,300italic,regular,italic,500,500italic,600,600italic,700,700italic,800,800italic,900,900italic');

  header {
      background-color: #191919;
      padding: 10px 0;
      text-align: center;
  }

  header h1 {
      margin: 0;
      color: #2163AD;
      font-family: 'Poppins', bold;
  }

  nav {
      margin: 10px;
  }

</style>