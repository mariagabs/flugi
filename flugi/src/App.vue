<template>
  <div id="app">
    <Header/>
    <SearchBar/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import SearchBar from "./components/SearchBar.vue";

export default {
  name: 'App',
  components: {
    Header,
    SearchBar
  }
}
</script>

<style lang="less">

* {
  border: 0;
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

a {
  text-decoration: none;
}

ul li {
  list-style: none;
}

body { 
  font-family: 'Quicksand', sans-serif;
  font-size: 14px;
}
</style>
