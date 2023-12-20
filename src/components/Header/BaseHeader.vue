<template>
  <div class="header-container">
    <header class="header">
      <a href="#default" class="logo">
        <img src="../../assets/logo.png" />
      </a>

      <div class="header-right">
        <a class="active" href="#home">Todos</a>
        <a href="#about">Água</a>
        <a href="#contact">Terra</a>
        <a href="#about">Fogo</a>
        <a href="#about">Ar</a>
      </div>
    </header>

    <div class="container">
      <h1 class="site-name">Pokédex</h1>

      <SearchBar />
    </div>
  </div>
</template>

<script>
import SearchBar from '../SearchBar/SearchBar.vue'

export default {
  name: 'BaseHeader',
  components: { SearchBar },
}
</script>

<style scoped>
header {
  padding: 0 24px;
}
.logo img {
  max-width: 240px;
}

.container {
  padding: 0 24px;
}

.site-name {
  font-size: 48px;
  font-weight: bold;
  color: #3965d2;
}

.header {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  height: 100%;
  background-color: #f1f1f1;
}

.header a {
  color: black;
  text-align: center;
  padding: 12px;
  text-decoration: none;
  font-size: 18px;
  line-height: 25px;
  border-radius: 4px;
}

.header a.logo {
  font-size: 25px;
  font-weight: bold;
}

.header a:hover {
  background-color: #ddd;
  color: black;
}

.header a.active {
  background-color: #3965d2;
  color: white;
}

@media screen and (max-width: 500px) {
  .header {
    flex-direction: column;
  }
  .header a {
    display: block;
  }

  .header-right {
    display: flex;
    flex-direction: row;
    padding-bottom: 24px;
  }
}
</style>
