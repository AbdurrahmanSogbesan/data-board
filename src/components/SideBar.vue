<template>
  <div class="sidebar-grid">
    <div class="sidebar">
      <div class="sidebar-items">
        <div class="sidebar-title">
          <Logo />
          <span class="bold-text ml-3">Data Board</span>
        </div>
        <SideBarItems />
      </div>
    </div>
    <div class="log-out">
      <div>Log Out</div>
    </div>
  </div>
</template>

<script>
import Logo from "./Logo";
import SideBarItems from "./SideBarItems";

export default {
  components: {
    Logo,
    SideBarItems
  }
};
</script>

<style lang="scss" scoped>
.sidebar-grid {
  background: #cb808d;
  height: 1024px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  width: 100%;
}

.sidebar {
  padding-top: 48px;
}

.sidebar-title {
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-left: 35px;
}

.bold-text {
  font-weight: bold;
  font-size: 16px;
  line-height: 19px;
  color: #ffffff;
}

.log-out {
  background: #15012e;
  width: 100%;
  color: #ffffff;
  height: 60px;
  align-items: center;
  display: flex;
  padding-left: 60px;
}
</style>
