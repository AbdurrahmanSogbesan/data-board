<template>
  <div id="app">
<<<<<<< HEAD
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
=======
    <div class="d-flex align-items-start">
      <SideBar />
      <!-- Replace below div with the header component here -->
      <Header />
>>>>>>> header-section
    </div>
  </div>
</template>

<script>
<<<<<<< HEAD
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
=======
  import SideBar from "./components/SideBar.vue";
  import Header from "./components/Header.vue";

  export default {
    name: "App",
    components: {
      SideBar,
      Header,
    },
  };
>>>>>>> header-section
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
