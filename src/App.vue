<template>
  <div id="app">
    <div class="row">
      <div class="col-2">
        <SideBar />
      </div>
      <div class="col-10"></div>
    </div>
  </div>
</template>

<script>
import SideBar from "./components/SideBar.vue";

export default {
  name: "App",
  components: {
    SideBar
  }
};
</script>

<style lang="scss"></style>
