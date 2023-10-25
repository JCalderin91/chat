<script setup>
defineProps({
  me: Boolean,
  message: String,
});
</script>

<template>
  <div :class="`message-container ${me ? 'me' : ''}`">
    <div class="message">{{ message }}</div>
    <small>10:35 pm</small>
  </div>
</template>

<style lang="scss" scoped>
.message-container {
  align-self: flex-start;
  margin-bottom: 0.5rem;
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
  }
  small {
    font-size: 0.6rem;
  }
}
</style>
