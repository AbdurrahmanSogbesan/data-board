<template>
  <div class="sidebar-item" :class="{ bold: link.isActive }">
    {{ link.text }}
  </div>
</template>

<script>
export default {
  props: {
    link: {
      type: Object
    },
    components: {}
  }
};
</script>

<style lang="scss" scoped>
.sidebar-item {
  font-weight: normal;
  font-size: 16px;
  line-height: 19px;
  color: #ffffff;
  display: flex;
  align-items: center;
  width: 100%;
  height: 60px;
  margin-bottom: 45px;
}

.sidebar-item.bold {
  font-weight: bold;
  border-right: 5px solid black;
}
</style>
