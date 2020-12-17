<template>
  <div class="sidebar-item" :class="{ active: link.isActive }">
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
  line-height: 19px;
  color: #ffffff;
  display: flex;
  align-items: center;
  width: 100%;
  height: 60px;
  margin-bottom: 45px;
  padding: 0 60px;
}

.sidebar-item.active {
  font-weight: bold;
  border-right: 5px solid#15012E;
}
</style>
