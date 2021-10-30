<template>
  <div class="home">
    <div class="sidebar bg-purple-700">
      <div
        class="
          rounded-lg
          shadow-xl
          bg-purple-500
          white
          flex flex-col
          items-center
          pt-2
          pr-2
          pl-3
          pb-3
          mt-4
          mr-4
          ml-4
        "
      >
        <h1 class="text-2xl font-bold text-white">$26,650</h1>
        <span class="text-white">current balance</span>
      </div>
      <div class="menu">
        <ul class="flex flex-col items-start pt-8 text-white">
          <li class="p-3">
            <i class="fa-solid fa-gauge-simple pr-3"></i><span>Dashboard</span>
          </li>
          <li class="p-3">
            <i class="fa-solid fa-chart-bar pr-3"></i><span>Charts</span>
          </li>
          <li class="p-3">
            <i class="fa-solid fa-calendar-days pr-3"></i><span>Calendar</span>
          </li>
          <li class="p-3">
            <i class="fa-solid fa-envelope pr-3"></i><span>Messages</span>
          </li>
          <li class="p-3">
            <i class="fa-solid fa-user pr-3"></i><span>User Profile</span>
          </li>
          <li class="p-3">
            <i class="fa-solid fa-gear pr-3"></i><span>settings</span>
          </li>
        </ul>
      </div>
    </div>
    <div class="main bg-gray-50">
      <div class="flex flex-col items-start pl-4"><CreditCard /></div>
    </div>
    <div class="aside bg-yellow-50"></div>
  </div>
</template>

<script>
// @ is an alias to /src
import CreditCard from "@/components/CreditCard.vue";

export default {
  name: "Home",
  components: {
    CreditCard,
  },
};
</script>

<style scoped>
.home {
  display: grid;
  grid-template-columns: 200px 1fr 300px;
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
