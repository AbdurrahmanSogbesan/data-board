<template>
  <tr class="table-row">
    <td colspan="2">{{ row.number }}</td>
    <td>{{ row.product }}</td>
    <td>{{ row.serial }}</td>
    <td>{{ row.stock }}</td>
    <td>{{ row.category }}</td>
    <td>{{ row.actions }}</td>
    <td>{{ row.dele }}</td>
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
  width: 100%;
  border: 1px solid #e2e8f0;

  td {
    font-size: 16px;
    line-height: 19px;
    color: #718096;
    padding: 24px 0;
    text-align: center;
  }
}
</style>
