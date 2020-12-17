<template>
  <div class="d-flex align-items-center header-section">
    <div class="d-flex align-items-center">
      <span class="header-title d-md-flex d-none">Dashboard Overview</span>
      <TextBox :icon="SearchIcon" placeholder="Search all..." />
    </div>
    <div class="d-flex align-items-center">
      <div class="d-md-flex d-none align-items-center">
        <HeaderListItems class="d-n" />
        <Button text="Download Client" class="d-n" />
      </div>
      <img src="@/assets/images/image.png" alt="" class="image ml-4" />
    </div>
  </div>
</template>

<script>
import TextBox from "./TextBox.vue";
import SearchIcon from "./SearchIcon.vue";
import HeaderListItems from "./HeaderListItems.vue";
import Button from "./Button.vue";

export default {
  data() {
    return {
      SearchIcon
    };
  },
  components: {
    TextBox,
    HeaderListItems,
    Button
  }
};
</script>

<style lang="scss" scoped>
.header-section {
  padding: 20px 22px;
  justify-content: space-between;
}
.header-title {
  font-size: 16px;
  color: #a0aec0;
  margin-right: 40px;
}
.image {
  border-radius: 25px;
}

.header-title {
  font-size: 16px;
  color: #a0aec0;
  margin-right: 40px;
}
.image {
  border-radius: 25px;
}
</style>
