<template>
  <li>
    <span>{{ todoItem }}</span>
    <button type="button" @click="removeItem">삭제</button>
  </li>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  props: {
    todoItem: {
      type: String,
      default: "",
    },
    index: {
      type: Number,
      default: 0,
    }
  },
  methods: {
    removeItem() {
      this.$emit('remove', this.index);
    },
  },
});
</script>

<style scoped></style>

