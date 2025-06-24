<script setup>
import Button from "../Button/Button.vue";
import IconLocation from "../../icons/IconLocation.vue";

const emit = defineEmits({
  selectCity(payload) {
    globalThis.console.log(`payload: ${payload}`);
    return payload;
  },
});

const select = () => {
  emit("selectCity", "Москва");
};
</script>

<template>
  <Button @click="select()">
    <template #iconLeft>
      <IconLocation />
    </template>

    Изменить город
  </Button>

  <input />
  <Button>Сохранить</Button>
</template>

<style scoped></style>
