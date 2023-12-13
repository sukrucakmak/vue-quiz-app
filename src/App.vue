<script setup>
import q from "./data/quizes.json"
import { ref } from "vue";

const quizes = ref(q)

</script>

<template>
  <div class="container">
    
    <header>
      <h1>Quizes</h1>
      <input type="text" placeholder="Search...">
    </header>
    <div class="cards">
      <div class="card" v-for="quiz in quizes" :key="quiz.id">
        <img :src="quiz.img" :alt="quiz.name">
        <div class="card-text">
          <h2> {{ quiz.name }}</h2>
          <p> {{ quiz.questions.length }} questions</p>
        </div>
      </div>
    </div>

  </div>
</template>

<style scoped>
.container {
  max-width: 1000px;
  margin: 0 auto;
}

.cards {
  display: flex;
  flex-wrap: wrap;
}

.card {
  width: 300px;
  overflow: hidden;
  border-radius: 2%;
  box-shadow: 0px 0px 2px #00000080;
  margin-bottom: 32px;
  margin-right: 16px;
  cursor: pointer;
  transition: 0.5s;
}

.card:hover {
  box-shadow: 0px 0px 16px #00000080;
}

.card img {
  width: 100%;
  height: 200px;
  margin: 0;
}

.card .card-text {
  padding: 0 0 8px 8px;
}

.card .card-text h2 {
  font-weight: bold;
}
</style>