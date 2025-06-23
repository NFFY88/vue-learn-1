<script setup></script>

<template>
  <button class="button">
    <slot name="icon-left"></slot>
    <slot></slot>
    <slot name="icon-right"></slot>
  </button>
</template>

<style scoped>
.button {
  appearance: none;
  border: none;
  padding: 14px;
  border-radius: 10px;
  background: var(--gradient-button);
  color: var(--color-text-primary);
  font-size: 20px;
  font-weight: 600;
  cursor: pointer;
  font-family: var(--font-primary);
}

.button:hover {
  background: var(--gradient-button-inverted);
}
</style>
