<template>
  <div class="sidebar-container">
    <div class="sidebar-title">
      <Logo />
      <span class="ml-3">Data Board</span>
    </div>
    <SideBarItems />
    <div class="log-out">
      Log Out
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
.sidebar-container {
  background: #cb808d;
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  height: 100vh;
  width: 17.5%;

  @media (max-width: 480px) {
    display: none;
  }
}

.sidebar-title {
  padding-top: 48px;
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-left: 35px;
  span {
    font-weight: bold;
    line-height: 19px;
    color: #ffffff;
  }
}

.log-out {
  background: #15012e;
  color: #ffffff;
  height: 60px;
  align-items: center;
  display: flex;
  padding-left: 60px;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
}
</style>
