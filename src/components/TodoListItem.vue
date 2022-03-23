<template>
  <li>{{ todoItem }}</li>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  props: {
    todoItem: {
      type: String,
      default: "",
    },
  },
});
</script>

<style scoped></style>

