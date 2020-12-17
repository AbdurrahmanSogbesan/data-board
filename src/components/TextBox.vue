<template>
  <div class="textbox">
    <input
      type="text"
      :placeholder="placeholder"
      :style="{ width: width, 'padding-left': paddingLeft }"
    />
    <component :is="icon" v-if="icon" class="icon"></component>
  </div>
</template>

<script>
export default {
  props: {
    icon: Object,
    placeholder: String,
    width: {
      type: String,
      default: "228px"
    },
    paddingLeft: {
      type: String,
      default: "40px"
    }
  }
};
</script>

<style lang="scss" scoped>
.textbox {
  position: relative;
  input {
    border: 1px solid #e2e8f0;
    border-radius: 4px;
    height: 40px;
    outline: none;

    &::placeholder {
      color: #cbd5e0;
      line-height: 19px;
    }
  }
}
.icon {
  position: absolute;
  top: 10px;
  left: 15px;
}
</style>
