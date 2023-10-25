<template>
  <section class="header">
    <div class="user-name">
      <div class="status"></div>
      <div class="name">Elizabeth Nelson</div>
    </div>
    <div class="actions">
      <button class="action">
        <font-awesome-icon icon="fa-phone" />
      </button>
      <button class="action">
        <font-awesome-icon icon="fa-video" />
      </button>
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
  .actions {
    display: flex;
    gap: 0.5rem;
    .action {
      border: none;
      height: 35px;
      width: 35px;
      border-radius: 50%;
      display: grid;
      place-items: center;
      background-color: var(--primary-color);
      color: white;
    }
  }
}
</style>
