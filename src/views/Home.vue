<template>
  <div class="home">Hello Budget App</div>
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
}
</style>
