<template>
  <div class="page-number ">
    <Arrow class="mr-4" />
    <span class="mr-2">1</span>
    <span class="active mr-2">2</span>
    <span class="mr-3">3</span>
    <span class="mr-3">4</span>
    <span>... 10</span>
    <Arrow class="rotate-right ml-4" />
  </div>
</template>

<script>
import Arrow from "./Arrow.vue";

export default {
  components: {
    Arrow
  }
};
</script>

<style lang="scss" scoped>
.page-number {
  padding: 24px 0;
  text-align: center;
  align-items: center;
  margin-left: 147px;

  @media (max-width: 480px) {
    left: 26%;
    position: absolute;
    margin-left: 0;
    padding-bottom: 8px;
  }

  span {
    font-size: 12px;
    color: #cbd5e0;
  }
}
.active {
  background-color: #15012e;
  color: #fff !important;
  border-radius: 30px;
  padding: 3px 6px;
}

.rotate-right {
  transform: rotate(-180deg);
}
</style>
