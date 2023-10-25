<template>
  <section class="form">
    <input type="text" placeholder="Type your message here..." />
    <div class="actions">
      <div class="action">
        <font-awesome-icon icon="fa-regular fa-face-smile" />
      </div>
      <div class="action">
        <font-awesome-icon icon="fa-paperclip" />
      </div>
      <div class="action primary">
        <font-awesome-icon icon="fa-paper-plane" />
      </div>
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
    .action {
      background-color: #ffffff50;
      height: 35px;
      width: 35px;
      display: grid;
      place-items: center;
      border-radius: 35px;
      &.primary {
        background-color: rgba(0, 31, 51, 1);
        color: white;
      }
    }
  }
}
</style>
