<template>
  <div id="app">
    <div class="d-flex align-items-start">
      <SideBar />
      <!-- Replace below div with the header component here -->
      <Header />
    </div>
  </div>
</template>

<script>
  import SideBar from "./components/SideBar.vue";
  import Header from "./components/Header.vue";

  export default {
    name: "App",
    components: {
      SideBar,
      Header,
    },
  };
</script>

<style lang="scss"></style>
