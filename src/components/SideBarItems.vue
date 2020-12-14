<template>
  <div class="sidebar-items">
    <SideBarItem
      :link="link"
      v-for="(link, index) in sideBarItems"
      :key="index"
    />
  </div>
</template>

<script>
  import SideBarItem from "./SideBarItem";

  export default {
    data() {
      return {
        sideBarItems: [
          { text: "Dashboard", isActive: true },
          { text: "User Management", isActive: false },
          { text: "Documents", isActive: false },
          { text: "Statistics", isActive: false },
          { text: "Settings", isActive: false },
        ],
      };
    },
    components: {
      SideBarItem,
    },
    props: {
      hasline: {
        type: Boolean,
        default: false,
      },
    },
  };
</script>

<style lang="scss" scoped>
  .sidebar-items {
    margin-top: 73px;
  }
</style>
