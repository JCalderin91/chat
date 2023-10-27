<script setup>
import IconButton from "@/components/atoms/IconButton.vue";
</script>
<template>
  <section class="form">
    <input type="text" placeholder="Type your message here..." />
    <div class="actions">
      <IconButton icon="fa-regular fa-face-smile" />
      <IconButton icon="fa-paperclip" />
      <IconButton color="primary" icon="fa-paper-plane" />
    </div>
  </section>
</template>

<style lang="scss" scoped>
.form {
  position: relative;
  input {
    height: 100%;
    width: calc(100% - 2rem);
    border: none;
    outline: none;
    background-color: #e9e9e9;
    padding: 0 1rem;
    display: block;
    color: #1b1b1b;
    padding-right: 7rem;
  }
  .actions {
    position: absolute;
    right: 1rem;
    top: 50%;
    transform: translateY(-50%);
    color: #333;
    display: flex;
    gap: 0.5rem;
  }
}
</style>
