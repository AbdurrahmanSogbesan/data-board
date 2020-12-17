<template>
  <tr class="table-row">
    <td align="left">{{ row.number }}</td>
    <td align="left">{{ row.product }}</td>
    <td align="left">{{ row.serial }}</td>
    <td align="left">{{ row.stock }}</td>
    <td align="left">{{ row.category }}</td>
    <td align="left" class="mobile-flex">
      Edit <span class="ml-4">Delete</span>
    </td>
  </tr>
</template>

<script>
export default {
  props: {
    row: {
      type: Object
    }
  }
};
</script>

<style lang="scss" scoped>
.table-row {
  border: 1px solid #e2e8f0;

  td {
    font-size: 16px;
    line-height: 19px;
    color: #718096;
    padding: 24px 37px;
  }
}

@media (max-width: 480px) {
  .mobile-flex {
    padding: 24px 0 !important;
  }
}
</style>
