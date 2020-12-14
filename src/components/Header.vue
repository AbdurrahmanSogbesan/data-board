<template>
  <div class="d-flex align-items-center">
    <span>Dashboard Overview</span>
    <TextBox :icon="SearchIcon" placeholder="Search all..." />
  </div>
</template>

<script>
import TextBox from "./TextBox.vue";
import SearchIcon from "./SearchIcon.vue";

export default {
  data() {
    return {
      SearchIcon
    };
  },
  components: {
    TextBox
  }
};
</script>

<style lang="scss" scoped></style>
