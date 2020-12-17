<template>
  <div class="d-flex">
    <HeaderListItem
      :link="link"
      v-for="(link, index) in HeaderListItems"
      :key="index"
    />
  </div>
</template>

<script>
import HeaderListItem from "./HeaderListItem.vue";
import InboxIcon from "./InboxIcon.vue";

export default {
  data() {
    return {
      HeaderListItems: [
        { text: "Help guides" },
        { text: "Inbox", icon: InboxIcon }
      ]
    };
  },
  components: {
    HeaderListItem
  }
};
</script>

<style lang="scss" scoped></style>
