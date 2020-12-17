<template>
  <div class="header-list-item d-flex">
    {{ link.text }} <component class="ml-1 mr-5" :is="link.icon"></component>
  </div>
</template>

<script>
export default {
  props: {
    link: Object
  }
};
</script>

<style lang="scss" scoped>
.header-list-item {
  color: #4a5568;
  margin-left: 38px;
  font-size: 12px;
}
</style>
