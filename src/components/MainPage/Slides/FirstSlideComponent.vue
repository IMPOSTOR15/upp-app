<template>

  <div class="main-wrapper">
    <!-- <img class="bg-svg" src="@/assets/mainPageImages/firstSlide/svgbg.svg" alt=""> -->
    <h1 class="header-title">Функционал</h1>
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
    <img class="bigdarkcircle" src="@/assets/mainPageImages/firstSlide/bigdarkcircle.svg" alt="">
    <img class="middarkcircle" src="@/assets/mainPageImages/firstSlide/middarkcircle.svg" alt="">
    <img class="circlepatern" src="@/assets/mainPageImages/firstSlide/circlepatern.svg" alt="">
    
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.main-wrapper {
  position: relative;
  display: flex;
  justify-content: center;
  min-width: 100%;
  background: #B1A9FF;
  flex-direction: column;
  margin: 0;
  height: 100vh;
}

.header-title {
  margin-left: auto;
  margin-right: auto;
  left: 0;
  right: 0;
  top: 10px;
  text-align: center;
  font-size: 40px;
  font-weight: bold;
  color: #fff;
  z-index: 2;
}

.function-container {
  background-color: #fff;
  border-radius: 20px;
  margin: 40px 14vw auto 14vw;
  display: flex;
  flex-direction: column;
  z-index: 1;
  
}
.top-row {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-between;
  padding-top: 50px;
  margin: 40px 5vw;
}

.bottom-row {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-between;
  padding-bottom: 50px;
  margin: 40px 5vw;
}

.bottom-card, .top-card {
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 200px;
  width: 200px;
  margin: auto;
  border-radius: 10px;
  cursor: pointer;
  -webkit-box-shadow: 0px 0px 10px 0px rgba(98, 83, 255, 0.38);
  -moz-box-shadow: 0px 0px 10px 0px rgba(98, 83, 255, 0.38);
  box-shadow: 0px 0px 10px 0px rgba(98, 83, 255, 0.38);
  transition: 0.5s all ease-in-out;
}
.bottom-card:hover, .top-card:hover {
  -webkit-box-shadow: 0px 0px 10px 5px rgba(98, 83, 255, 0.38);
  -moz-box-shadow: 0px 0px 10px 5px rgba(98, 83, 255, 0.38);
  box-shadow: 0px 0px 10px 5px rgba(98, 83, 255, 0.38);
}

.bigdarkcircle {
  position: absolute;
  width: 370px;
  height: 370px;
  top: 50px;
  left: 115px;
}

.middarkcircle {
  position: absolute;
  width: 240px;
  height: 240px;
  bottom: 100px;
  left: 600px;
}

.circlepatern {
  position: absolute;
  width: 570px;
  height: 240px;
  bottom: 100px;
  right: 120px;
}

@media (max-width: 1200px) {
  .main-wrapper {
    height: auto;
    margin-top: 320px; 
    /* !!!!!Тут надо подумать!!!! */
  }
  .middarkcircle {

    left: auto;
    right: 0px;
  }
  .bigdarkcircle {
    left: 0px;
  }
  .function-container {
    margin-top: 50px;
    margin-bottom: 50px;
  }
  .top-row {
    padding-top: 0;
    margin: 40px 2vw 0 2vw;
  }

  .bottom-row {
    padding-bottom: 0;
    margin: 0 2vw 40px 2vw;
  }
  .bottom-card, .top-card {

    margin: 10px auto;

  }
}
@media (max-width: 980px) {

}  
</style>