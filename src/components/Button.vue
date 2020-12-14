<template>
  <div>
    <button
      :style="{
        width: width,
        height: height,
        'background-color': backgroundColor,
        'font-size': fontSize
      }"
    >
      {{ text }}
    </button>
  </div>
</template>

<script>
export default {
  props: {
    width: {
      type: String,
      default: "101px"
    },
    height: {
      type: String,
      default: "30px"
    },
    backgroundColor: {
      type: String,
      default: "#CB808D"
    },
    fontSize: {
      type: String,
      default: "12px"
    },
    text: String
  }
};
</script>

<style lang="scss" scoped>
button {
  border-radius: 4px;
  outline: none;
  color: #f7fafc;
  border: none;
}
</style>
