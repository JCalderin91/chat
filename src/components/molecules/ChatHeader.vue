<template>
  <section class="header">
    <div class="user-name">
      <div class="status"></div>
      <div class="name">Elizabeth Nelson</div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
  .user-name {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 1rem;
    .status {
      height: 10px;
      width: 10px;
      border-radius: 10px;
      background-color: #01c421;
    }
    .name {
      font-size: 1.5rem;
      color: #333;
      font-weight: 600;
    }
  }
}
</style>
