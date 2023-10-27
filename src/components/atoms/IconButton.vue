<script setup>
defineProps({
  icon: String,
  color: {
    validator(value) {
      return ["primary", "secondary"].includes(value);
    },
  },
});
</script>

<template>
  <button type="button" :class="color">
    <font-awesome-icon :icon="icon" />
  </button>
</template>

<style lang="scss" scoped>
button {
  background-color: #ffffff50;
  height: 35px;
  width: 35px;
  display: grid;
  place-items: center;
  border-radius: 35px;
  border: none;
  &:hover {
    background-color: #cfcfcf77;
  }
  &.primary {
    background-color: rgba(0, 31, 51, 1);
    color: white;
    &:hover {
      background-color: rgb(2, 55, 90);
    }
  }
}
</style>
