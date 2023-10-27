<script setup>
import UserPicture from "@/components/atoms/UserPicture.vue";
defineProps({
  name: String,
  resume: String,
});
</script>

<template>
  <article class="contact">
    <UserPicture />
    <div class="contact-info">
      <h6 class="name">{{ name }}</h6>
      <small class="resume">{{ resume }}</small>
      <div class="counter">1</div>
    </div>
  </article>
</template>

<style lang="scss" scoped>
.contact {
  padding: 0.5rem 1.5rem;
  gap: 0.5rem;
  display: flex;
  align-items: center;
  cursor: pointer;
  &:hover {
    background-color: #ffffff21;
  }
  .contact-info {
    position: relative;
    flex: 1;
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
    .counter {
      position: absolute;
      right: 0.5rem;
      top: 50%;
      transform: translateY(-50%);
      width: 16px;
      height: 16px;
      border-radius: 50%;
      background-color: #fff;
      color: #333;
      display: grid;
      place-items: center;
      font-size: 10px;
      font-weight: 600;
      line-height: 1;
    }
  }
}
</style>
