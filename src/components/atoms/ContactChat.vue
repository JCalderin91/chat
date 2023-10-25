<script setup>
defineProps({
  name: String,
  resume: String,
});
</script>

<template>
  <div class="contact">
    <h6 class="name">{{ name }}</h6>
    <small class="resume">{{ resume }}</small>
  </div>
</template>

<style lang="scss" scoped>
.contact {
  padding: 0.5rem 1.5rem;
  &:hover {
    background-color: #ffffff21;
  }
  .name {
    font-size: 1rem;
    line-height: 1.1;
    color: #ffffff;
  }
  .resume {
    font-size: 0.8rem;
    line-height: 1.1;
    color: #cacaca;
  }
}
</style>
