<template>
  <div class="container">
    <header>
      <h1>Quizes</h1>
      <input type="text" placeholder="Search...">
    </header>
    <div class="cards">
      <div class="card">
        <img src="https://miro.medium.com/v2/resize:fit:1400/1*L76A5gL6176UbMgn7q4Ybg.jpeg" alt="Math">
        <div class="card-text">
          <h2>Math</h2>
          <p>15 questions</p>
        </div>
      </div>
      <div class="card">
        <img src="https://miro.medium.com/v2/resize:fit:1400/1*L76A5gL6176UbMgn7q4Ybg.jpeg" alt="Math">
        <div class="card-text">
          <h2>Math</h2>
          <p>15 questions</p>
        </div>
      </div>
      <div class="card">
        <img src="https://miro.medium.com/v2/resize:fit:1400/1*L76A5gL6176UbMgn7q4Ybg.jpeg" alt="Math">
        <div class="card-text">
          <h2>Math</h2>
          <p>15 questions</p>
        </div>
      </div>
      <div class="card">
        <img src="https://miro.medium.com/v2/resize:fit:1400/1*L76A5gL6176UbMgn7q4Ybg.jpeg" alt="Math">
        <div class="card-text">
          <h2>Math</h2>
          <p>15 questions</p>
        </div>
      </div>
      <div class="card">
        <img src="https://miro.medium.com/v2/resize:fit:1400/1*L76A5gL6176UbMgn7q4Ybg.jpeg" alt="Math">
        <div class="card-text">
          <h2>Math</h2>
          <p>15 questions</p>
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
  box-shadow: 0px 0px 10px #00000080;
  transform: scaleX(1.05) scaleY(1.05);

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