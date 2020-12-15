<template>
  <div class="table d-flex flex-column align-items-align-items-baseline">
    <div class="table-header d-flex align-items-baseline">
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
    <table>
      <tbody>
        <tr class="table-top">
          <th colspan="2">#</th>
          <th>Product</th>
          <th>Serial Code</th>
          <th>Stock</th>
          <th>Category</th>
          <th colspan="2">Actions</th>
        </tr>
        <TableRow v-for="(row, index) in rows" :key="index" :row="row" />
      </tbody>
    </table>
    <div class="d-flex align-items-baseline justify-content-between px-4">
      <div></div>
      <PageNumber />
      <Select />
    </div>
  </div>
</template>

<script>
import Button from "./Button.vue";
import TextBox from "./TextBox.vue";
import SearchIcon from "./SearchIcon.vue";
import FilterIcon from "./FilterIcon.vue";
import TableRow from "./TableRow.vue";
import PageNumber from "./PageNumber.vue";
import Select from "./Select.vue";

export default {
  data() {
    return {
      SearchIcon,
      rows: [
        {
          number: "03",
          product: "Macbook pro 16",
          serial: "#123-456ABC",
          stock: "123",
          category: "Apple",
          actions: "Edit",
          delete: "Delete"
        },
        {
          number: "03",
          product: "Macbook pro 16",
          serial: "#123-456ABC",
          stock: "123",
          category: "Apple",
          actions: "Edit",
          delete: "Delete"
        },
        {
          number: "03",
          product: "Macbook pro 16",
          serial: "#123-456ABC",
          stock: "123",
          category: "Apple",
          actions: "Edit",
          delete: "Delete"
        },
        {
          number: "03",
          product: "Macbook pro 16",
          serial: "#123-456ABC",
          stock: "123",
          category: "Apple",
          actions: "Edit",
          delete: "Delete"
        },
        {
          number: "03",
          product: "Macbook pro 16",
          serial: "#123-456ABC",
          stock: "123",
          category: "Apple",
          actions: "Edit",
          delete: "Delete"
        },
        {
          number: "03",
          product: "Macbook pro 16",
          serial: "#123-456ABC",
          stock: "123",
          category: "Apple",
          actions: "Edit",
          delete: "Delete"
        },
        {
          number: "03",
          product: "Macbook pro 16",
          serial: "#123-456ABC",
          stock: "123",
          category: "Apple",
          actions: "Edit",
          delete: "Delete"
        },
        {
          number: "03",
          product: "Macbook pro 16",
          serial: "#123-456ABC",
          stock: "123",
          category: "Apple",
          actions: "Edit",
          delete: "Delete"
        },
        {
          number: "03",
          product: "Macbook pro 16",
          serial: "#123-456ABC",
          stock: "123",
          category: "Apple",
          actions: "Edit",
          delete: "Delete"
        },
        {
          number: "03",
          product: "Macbook pro 16",
          serial: "#123-456ABC",
          stock: "123",
          category: "Apple",
          actions: "Edit",
          delete: "Delete"
        }
      ]
    };
  },
  components: {
    Button,
    TextBox,
    FilterIcon,
    TableRow,
    PageNumber,
    Select
  }
};
</script>

<style lang="scss" scoped>
.table {
  background-color: #fff;
  border-radius: 5px;
  width: 100%;
}

.table-header {
  padding: 23px 20px 21px 37px;
  justify-content: space-between;
}

.order-catalogue {
  font-size: 20px;
  line-height: 23px;
  color: #4a5568;
  margin-right: 8px;
}

table {
  border-collapse: collapse !important;
}

.table-top {
  background-color: #edf2f7;
  width: 100%;

  th {
    font-weight: normal;
    padding: 11px 37px;
    font-size: 16px;
    line-height: 19px;
    color: #4a5568;
    border: none;
  }
}
</style>
