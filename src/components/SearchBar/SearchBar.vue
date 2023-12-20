<template>
  <div class="search-container">
    <input class="search-input" placeholder="Digite sua pesquisa" />
    <button class="search-button">Pesquisar</button>
  </div>
</template>

<!--  -->
<script>
export default {
  name: 'SearchBar',
}
</script>

<style>
.search-container {
  display: flex;
  align-items: center;
}

.search-input {
  width: 100%;
  padding: 24px;
  border: 2px solid #3965d2;
  border-radius: 5px 0 0 5px;
  margin-right: -1px;
}

.search-button {
  padding: 25px;
  background-color: #3965d2;
  color: #fff;
  border: 1px solid #3965d2;
  border-radius: 0 5px 5px 0;
  cursor: pointer;
}
</style>
