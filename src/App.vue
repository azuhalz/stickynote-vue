<script setup></script>

<template>
  <main>
    <div class="container">
      <header>
        <h1 class="header-title">Memo</h1>
        <button class="header-button">+</button>
      </header>

      <div class="card-container">
        <div class="card">
          <p class="card-content">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Asperiores
            alias, blanditiis deserunt sapiente consequuntur dignissimos aperiam
            fugit, quos maxime aliquam modi explicabo velit placeat tempora
            tenetur.
          </p>
          <p class="card-date">12/12/2026</p>
        </div>

        <div class="card">
          <p class="card-content">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Asperiores
            alias, blanditiis deserunt sapiente consequuntur dignissimos aperiam
            fugit, quos maxime aliquam modi explicabo velit placeat tempora
            tenetur.
          </p>
          <p class="card-date">12/12/2026</p>
        </div>

        <div class="card">
          <p class="card-content">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Asperiores
            alias, blanditiis deserunt sapiente consequuntur dignissimos aperiam
            fugit, quos maxime aliquam modi explicabo velit placeat tempora
            tenetur.
          </p>
          <p class="card-date">12/12/2026</p>
        </div>
      </div>
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

.card {
  width: 225px;
  height: 225px;
  background-color: #495a7d;
  padding: 10px;
  background-color: pink;
  margin-bottom: 20px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.card-container {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
}
</style>
