<template>
  <div class="parent-container">
    <h2>Slots in Option API</h2>
    <h3>Parent Component</h3>
    <ChildComponent>
      <template v-slot:title>
        Child Title <span class="accent">(from slot)</span>
      </template>
      <template v-slot:content>
        Child Content <span class="accent">(from slot):</span> Lorem ipsum dolor
        sit amet consectetur adipisicing elit. Rerum, molestiae? Ea consectetur
        nobis quae, dolores iste repellat est nostrum non?
      </template>
    </ChildComponent>
  </div>
</template>

<script>
import ChildComponent from "./ChildComponent.vue";

export default {
  components: { ChildComponent },
};
</script>

<style scoped></style>