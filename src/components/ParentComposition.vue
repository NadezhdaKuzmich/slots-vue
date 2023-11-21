<template>
  <div class="parent-container">
    <h2>Slots in Composition API</h2>
    <h3>Parent Component</h3>
    <ChildComposition>
      <template v-slot:title>
        Child Title <span class="accent">(from slot)</span>
      </template>
      <p>
        Child Content <span class="accent">(from slot):</span> Lorem ipsum dolor
        sit amet consectetur adipisicing elit. Rerum, molestiae? Ea consectetur
        nobis quae, dolores iste repellat est nostrum non?
      </p>
    </ChildComposition>
  </div>
</template>

<script>
import ChildComposition from "./ChildComposition.vue";
import { defineComponent } from "vue";

export default defineComponent({
  name: "ParentComposition",
  components: { ChildComposition },
  setup() {
    return {};
  },
});
</script>

<style scoped></style>