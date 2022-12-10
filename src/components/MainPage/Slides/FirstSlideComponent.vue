<template>
  <div class="main-wrapper">
    <!-- <img class="bg-svg" src="@/assets/mainPageImages/firstSlide/svgbg.svg" alt=""> -->
    <h1>Функционал</h1>
    <div class="function-container">
      <div class="top-row">
        <div class="top-card">
          <div class="img-wrapper">
            <img src="@/assets/mainPageImages/firstSlide/calculator.svg" alt="">
          </div>
          <p class="card-text">Калькуляторы</p>
        </div>
        <div class="top-card">
          <div class="img-wrapper">
            <img src="@/assets/mainPageImages/firstSlide/products.svg" alt="">
          </div>
          <p class="card-text">Продукты</p>
        </div>
        <div class="top-card">
          <div class="img-wrapper">
            <img src="@/assets/mainPageImages/firstSlide/excersises.svg" alt="">
          </div>
          <p class="card-text">Упражнения</p>
        </div>
      </div>
      <div class="bottom-row">
        <div class="bottom-card">
          <div class="img-wrapper">
            <img src="@/assets/mainPageImages/firstSlide/calculatorcallory.svg" alt="">
          </div>
          <p class="card-text">Калькулятор калорий</p>
        </div>
        <div class="bottom-card">
          <div class="img-wrapper">
            <img src="@/assets/mainPageImages/firstSlide/idealweight.svg" alt="">
          </div>
          <p class="card-text">Идеальный вес</p>
        </div>
        <div class="bottom-card">
          <div class="img-wrapper">
            <img src="@/assets/mainPageImages/firstSlide/calculatorimt.svg" alt="">
          </div>
          <p class="card-text">Расчет ИМТ тела</p>
        </div>
        <div class="bottom-card">
          <div class="img-wrapper">
            <img src="@/assets/mainPageImages/firstSlide/metabolism.svg" alt="">
          </div>
          <p class="card-text">Обмен веществ</p>
        </div>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.main-wrapper {
  display: flex;
  justify-content: center;
  margin: auto;
  min-width: 100%;
  /* background: #B1A9FF; */
  background: #B1A9FF url(@/assets/mainPageImages/firstSlide/svgbg.svg); /* Фоновый цвет и фоновый рисунок*/
  flex-direction: column;
  margin: 0;
  height: 100vh;
}

.function-container {
  background-color: #fff;
  border-radius: 20px;
  margin: 0 10vw;
  display: flex;
  flex-direction: column;
  
}
.top-row {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding-top: 80px;
  margin: 40px 10vw;
  
}

.bottom-row {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding-bottom: 80px;
  margin: 40px 10vw;
}

.bottom-card, .top-card {
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 200px;
  width: 200px;
  margin: auto;
  border-radius: 10px; 
  -webkit-box-shadow: 0px 5px 24px -4px rgba(65, 0, 90, 0.39);
  -moz-box-shadow: 0px 5px 24px -4px rgba(65, 0, 90, 0.39);
  box-shadow: 0px 5px 24px -4px rgba(65, 0, 90, 0.39);
}
</style>