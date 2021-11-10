<template>
  <div class="search-bar">
      <div class="container">
      </div>
  </div>
</template>

<script>
export default {
    name: 'SearchBar'
}
</script>

<style lang="less" scoped>
@import "../assets/variables.less";

.search-bar {
    top: @height-menu-desktop;
    height: @height-search-bar-desktop;
    background-color: @orange;

    .container { 
        margin-left: @margin-body-desktop;
        margin-right: @margin-body-desktop;
    }
}
</style>