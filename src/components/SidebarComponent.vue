<template>
  <div class="sidebar">
    <h3>Liens utiles</h3>
    <ul>
      <li><a href="#">Accueil</a></li>
      <li><a href="#">Articles</a></li>
      <li><a href="#">À propos</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'SidebarComponent'
}
</script>

<style scoped>
.sidebar {
  background-color: #f2f2f2;
  padding: 20px;
}

h3 {
  margin-bottom: 10px;
}

ul {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: center;

    justify-content: center;
    list-style-type: none;
    padding: 0;
}

li {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    margin-bottom: 5px;
}

a {
  text-decoration: none;
  color: #333;
  margin: 10px;
}

a:hover {
  color: #666;
}
</style>
