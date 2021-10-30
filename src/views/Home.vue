<template>
  <div class="home">
    <div class="sidebar">Sidebar</div>
    <div class="main">Content</div>
    <div class="aside">Side</div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: {},
};
</script>

<style scoped>
.home {
  display: grid;
  grid-template-columns: 150px 1fr 200px;
  grid-template-rows: repeat(5, 1fr);
  grid-column-gap: 3px;
  grid-row-gap: 0px;
  min-height: 100vh;
  min-width: 100vw;
}
</style>
