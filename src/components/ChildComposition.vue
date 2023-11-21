<template>
  <div class="child-container">
    <h3><slot name="title"></slot></h3>
    <slot></slot>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "ChildComposition",
  setup() {
    return {};
  },
});
</script>

<style scoped></style>