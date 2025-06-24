<script setup>
const { label, value } = defineProps({
    label: String,
    value: String
});
</script>

<template>
  <div class="stat">
    <span class="stat-title">{{ label }}</span>
    <span class="stat-value">{{ value }}</span>
  </div>
</template>

<style scoped>
.stat {
  display: flex;
  align-items: center;
  justify-content: space-between;
  color: var(--color-text-primary);
  font-size: 28px;
  gap: 10px;
}

.stat-title {
  font-weight: 700;
  text-transform: uppercase;
}

.stat-value {
  font-weight: 500;
}
</style>
