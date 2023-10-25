<script setup>
import UserPicture from "@/components/atoms/UserPicture.vue";
defineProps({
  me: Boolean,
  message: String,
});
</script>

<template>
  <div :class="`message-container ${me ? 'me' : ''}`">
    <div class="user-info">
      <UserPicture />
      <small>10:35 pm</small>
    </div>
    <div class="message">
      {{ message }} <font-awesome-icon icon="fa-solid fa-user-secret" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.message-container {
  align-self: flex-start;
  margin-bottom: 0.5rem;
  display: flex;
  align-items: flex-end;
  gap: 0.5rem;
  .user-info {
    display: flex;
    flex-direction: column;
  }
  &.me {
    text-align: right;
    align-self: flex-end;
    .message {
      background-color: rgba(0, 31, 51, 1);
      border-radius: 0.6rem 0.6rem 0 0.6rem;
    }
  }

  .message {
    padding: 0.6rem;
    border-radius: 0.6rem 0.6rem 0.6rem 0;
    background-color: #777777;
    color: white;
    margin-bottom: 2.5rem;
  }
  small {
    font-size: 0.6rem;
  }
}
</style>
