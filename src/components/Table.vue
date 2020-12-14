<template>
  <div class="table d-flex flex-column align-items-align-items-baseline">
    <div class="table-head d-flex align-items-baseline">
      <div class="d-flex align-items-baseline">
        <span class="order-catalogue">Order Catalogue</span>
        <Button
          width="67px"
          height="20px"
          backgroundColor="#4FD1C5"
          fontSize="11px"
          text="New Items"
        />
      </div>

      <div class="d-flex align-items-baseline">
        <TextBox
          placeholder="Select column"
          paddingLeft="15px"
          width="178px"
          class="mr-5"
        />
        <TextBox placeholder="Select list..." :icon="SearchIcon" class="mr-3" />
        <FilterIcon class="mr-3" />
        <Button width="91px" height="40px" fontSize="16px" text="Add new" />
      </div>
    </div>
  </div>
</template>

<script>
import Button from "./Button.vue";
import TextBox from "./TextBox.vue";
import SearchIcon from "./SearchIcon.vue";
import FilterIcon from "./FilterIcon.vue";

export default {
  data() {
    return {
      SearchIcon
    };
  },
  components: {
    Button,
    TextBox,
    FilterIcon
  }
};
</script>

<style lang="scss" scoped>
.table {
  background-color: #fff;
  border-radius: 5px;
}

.table-head {
  padding: 23px 20px 21px 37px;
  justify-content: space-between;
}

.order-catalogue {
  font-size: 20px;
  line-height: 23px;
  color: #4a5568;
  margin-right: 8px;
}
</style>
