<template>
  <div id="app">
    <div class="d-flex ">
      <SideBar />
      <!-- Replace below div with the header component here -->
      <div class="table-section">
        <div class="app-header">
          <Header />
        </div>
        <section class="grey-background">
          <Table />
        </section>
      </div>
    </div>
  </div>
</template>

<script>
import SideBar from "./components/SideBar.vue";
import Header from "./components/Header.vue";
import Table from "./components/Table.vue";

export default {
  name: "App",
  components: {
    SideBar,
    Header,
    Table
  }
};
</script>

<style lang="scss">
.table-section {
  width: 83%;
}
.grey-background {
  background-color: #eeecec;
  padding: 20px;
  width: 100%;
}
</style>
