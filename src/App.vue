<script setup>
import { ref } from "vue";

const showForm = ref(false);
</script>

<template>
  <main>
    <div class="container">
      <header>
        <h1 class="header-title">Memo</h1>
        <button class="header-button" @click="showForm = true">+</button>
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

    <div v-if="showForm" class="form-overlay">
      <div class="form-modal">
        <button class="form-close-btn">x</button>
        <textarea name="memo" id="memo" cols="30" rows="10"></textarea>
        <button class="form-save-btn">Save</button>
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

.form-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.77);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 10;
}

.form-modal {
  width: 420px;
  background-color: white;
  border-radius: 10px;
  padding: 30px;
  position: relative;
  display: flex;
  flex-direction: column;
}

.form-save-btn {
  padding: 10px 20px;
  font-size: 20px;
  width: 100%;
  background-color: #495a7d;
  color: white;
  border: none;
  cursor: pointer;
  border-radius: 5px;
  margin-top: 15px;
}

.form-close-btn {
  position: absolute;
  top: 2px;
  right: 3px;
  width: 30px;
  height: 30px;
  background-color: transparent;
  border: none;
  font-size: 25px;
  cursor: pointer;
}
</style>
