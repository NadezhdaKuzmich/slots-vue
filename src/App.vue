<template>
  <div class="container">
    <h1>Option/Composition API. Slots.</h1>
    <div class="components">
      <ParentComponent />
      <ParentComposition />
    </div>
  </div>
</template>

<script>
import ParentComponent from "./components/ParentComponent.vue";
import ParentComposition from "./components/ParentComposition.vue";

export default {
  components: { ParentComponent, ParentComposition },
};
</script>

<style>
body {
  font-size: 18px;
  color: #38393f;
  margin: 0;
}

.container {
  max-width: 1000px;
  padding: 20px;
  margin: auto;
}

h1,
h2 {
  text-align: center;
}

.components {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 40px 0;
  gap: 20px;
}

.accent {
  font-size: 14px;
  font-weight: 300;
  opacity: 0.8;
}

.parent-container {
  max-width: 580px;
  color: #fff;
  background: #4a6654;
  border: 4px solid #1c3f24;
  border-radius: 8px;
  padding: 10px 20px 30px;
}

.parent-container h2 {
  margin-bottom: 30px;
}
</style>