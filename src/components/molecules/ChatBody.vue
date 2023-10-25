<script setup>
import Message from "@/components/atoms/Message.vue";
</script>
<template>
  <section class="chat-body">
    <Message message="Hola, como estas?" />
    <Message me message="Bien y tu?" />
    <Message message="Bien" />
  </section>
</template>
<style lang="scss" scoped>
.chat-body {
  color: #333;
  background-color: #f2fffc;
  padding: 0.2rem 1rem;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
}
</style>
