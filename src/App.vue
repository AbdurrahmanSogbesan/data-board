<template>
  <div id="app">
    <div class="d-flex">
      <SideBar />
      <!-- Replace below div with the header component here -->
      <div class="app-header">
        <Header />
      </div>
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
    Header
  }
};
</script>

<style lang="scss"></style>
