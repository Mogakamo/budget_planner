<template>
  <div class="home">
    <div class="sidebar bg-indigo-700">
      <div
        class="
          rounded-lg
          shadow-xl
          bg-blue-200
          white
          content-center
          pt-2
          pr-2
          pl-3
          pb-3
          text-lg
          mt-4
          mr-4
          ml-4
        "
      >
        <h1>$26,650</h1>
        <span>current balance</span>
      </div>
    </div>
    <div class="main bg-gray-200">Content</div>
    <div class="aside bg-yellow-200">Side</div>
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
  grid-template-columns: 230px 1fr 300px;
  grid-template-rows: repeat(5, 1fr);
  min-height: 100vh;
  min-width: 100vw;
}

.sidebar {
  border: transparent;
  grid-row-start: 1;
  grid-row-end: 6;
}

.main {
  border: transparent;
  grid-row-start: 1;
  grid-row-end: 6;
  border-top-left-radius: 50%b;
}

.aside {
  border: transparent;
  grid-row-start: 1;
  grid-row-end: 6;
}
</style>
