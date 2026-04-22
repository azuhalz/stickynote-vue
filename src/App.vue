<script setup></script>

<template>
  <main>
    <div class="container">
      <header>
        <h1 class="header-title">Memo</h1>
        <button class="header-button">+</button>
      </header>

      <div>card</div>
    </div>
  </main>
</template>

<style scoped>
main {
  height: 100vh;
  width: 100vw;
}

.container {
  max-width: 900px;
  padding: 10px;
  margin: 0 auto;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.header-title {
  font-size: 48px;
  font-weight: bold;
  margin-bottom: 25px;
  color: #495a7d;
}

.header-button {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background-color: #495a7d;
  color: white;
  font-size: 24px;
  border: none;
  cursor: pointer;
}
</style>
