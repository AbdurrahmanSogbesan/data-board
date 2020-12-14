<template>
  <div id="app">
    <div class="d-flex">
      <SideBar />
      <!-- Replace below div with the header component here -->
      <div class="app-header"></div>
    </div>
  </div>
</template>

<script>
  import SideBar from "./components/SideBar.vue";

  export default {
    name: "App",
    components: {
      SideBar,
    },
  };
</script>

<style lang="scss"></style>
