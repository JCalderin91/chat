<script setup>
import UserPicture from "@/components/atoms/UserPicture.vue";
defineProps({
  name: String,
  resume: String,
});
</script>

<template>
  <div class="contact">
    <UserPicture />
    <div class="contact-info">
      <h6 class="name">{{ name }}</h6>
      <small class="resume">{{ resume }}</small>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.contact {
  padding: 0.5rem 1.5rem;
  gap: 0.5rem;
  display: flex;
  align-items: center;
  &:hover {
    background-color: #ffffff21;
  }
  .contact-info {
    .name {
      font-size: 1rem;
      line-height: 1.1;
      color: #ffffff;
    }
    .resume {
      font-size: 0.8rem;
      line-height: 1.1;
      color: #cacaca;
      padding: 0;
      margin: 0;
    }
  }
}
</style>
