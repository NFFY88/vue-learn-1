<script setup>
import CitySelect from "./components/CitySelect/CitySelect.vue";
import Stat from "./components/Stat/Stat.vue";

const data = {
  label: "Влажность",
  value: "80%",
};

const selectCity = (payload) => {
  globalThis.console.log(`selectCity: ${payload}`);
};
</script>

<template>
  <main class="main">
    <Stat v-bind="data" />
    <Stat label="Осадки" value="0%" />
    <CitySelect @select-city="selectCity" />
  </main>
</template>

<style scoped>
.main {
  padding: 60px 50px;
  border-radius: 25px;
  background-color: var(--color-bg-content);
}
</style>
