<script setup>
import ContactList from "@/components/organisms/ContactList.vue";
import ChatBody from "@/components/molecules/ChatBody.vue";
import ChatHeader from "@/components/molecules/ChatHeader.vue";
import ChatForm from "@/components/molecules/ChatForm.vue";
</script>

<template>
  <main>
    <aside>
      <div class="header">
        <div class="app-name">Chat</div>
      </div>
      <div class="contacts">
        <div class="search">
          <input type="text" placeholder="Search here..." />
        </div>
        <ContactList />
      </div>
    </aside>
    <section class="main">
      <ChatHeader />
      <ChatBody />
      <ChatForm />
    </section>
  </main>
</template>

<style lang="scss" scoped>
main {
  display: grid;
  grid-template-columns: 400px 1fr;
  min-height: calc(100vh - 4rem);
  min-width: 1200px;
  margin: 0 auto;
  margin: 2rem;
  background-color: #e9e9e9;
  border-radius: 0.4rem;
  aside {
    background-color: #258888;
    border-radius: 0.4rem;
    .header {
      padding: 1rem;
      .app-name {
        font-size: 1.4rem;
        font-weight: 600;
      }
    }
    .search {
      padding: 1rem;
      margin-bottom: 1rem;
      input {
        width: 100%;
        padding: 0.8rem 1rem;
        border-radius: 0.3rem;
        background-color: #3cc4c4;
        color: #333;
        border: none;
        outline: none;
      }
    }
  }
  .main {
    display: grid;
    grid-template-rows: 80px 1fr 60px;
  }
}
</style>
