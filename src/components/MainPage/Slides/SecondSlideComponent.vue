<template>
  <div class="main-wrapper">
    <div class="left-block">
      <div class="content-block">
        <div class="text-block">
          <h1>Продукты</h1>
          <p>Полезные продукты из магазина</p>
        </div>
      </div>
    </div>
    <div class="right-block">
      <div class="images-wrapper">
        <div class="img-card">
          <img class="image" src="@/assets/mainPageImages/secondSlide/cards/first.png" alt="">
          <div class="card-block">
            <div class="card-top-block"></div>
            <div class="card-bottom-block">
              <p class="card-text">Фрукты</p>
            </div>
          </div>
        </div>
        <div class="img-card">
          <img class="image" src="@/assets/mainPageImages/secondSlide/cards/second.png" alt="">
          <div class="card-block">
            <div class="card-top-block"></div>
            <div class="card-bottom-block">
              <p class="card-text">Рыба</p>
            </div>
          </div>
        </div>
        <div class="img-card">
          <img class="image" src="@/assets/mainPageImages/secondSlide/cards/third.png" alt="">
          <div class="card-block">
            <div class="card-top-block"></div>
            <div class="card-bottom-block">
              <p class="card-text">Орехи</p>
            </div>
          </div>
        </div>
        <div class="img-card">
          <img class="image" src="@/assets/mainPageImages/secondSlide/cards/fourth.png" alt="">
          <div class="card-block">
            <div class="card-top-block"></div>
            <div class="card-bottom-block">
              <p class="card-text">Яйца и молочные</p>
            </div>
          </div>
        </div>
        <div class="img-card">
          <img class="image" src="@/assets/mainPageImages/secondSlide/cards/fifth.png" alt="">
          <div class="card-block">
            <div class="card-top-block"></div>
            <div class="card-bottom-block">
              <p class="card-text">Мясо птицы</p>
            </div>
          </div>
        </div>
        <div class="img-card">
          <img class="image" src="@/assets/mainPageImages/secondSlide/cards/sixth.png" alt="">
          <div class="card-block">
            <div class="card-top-block"></div>
            <div class="card-bottom-block">
              <p class="card-text">Полезные завтраки</p>
            </div>
          </div>
        </div>
      </div>
      <div class="button-wrapper">
        <button class="recipes-btn">Смотреть рецепты</button>
      </div>
    </div>
    <img class="bigcircle" src="@/assets/mainPageImages/secondSlide/bigcircle.svg" alt="">
    <img class="mediumcircle" src="@/assets/mainPageImages/secondSlide/mediumcircle.svg" alt="">
    <img class="smallcircle" src="@/assets/mainPageImages/secondSlide/smallcircle.svg" alt="">
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.main-wrapper {
  position: relative;
  background-color: #fff;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  height: 100vh;
  margin: 70px auto 0 auto;
  max-width: 79vw;
}
.left-block {
  display: flex;
  justify-content: center;
  width: 2050px;
  height: 800px;
  background-image: url(@/assets/mainPageImages/secondSlide/productsblockbg.png);
  background-repeat: no-repeat;
  margin: 7vh 0;
  border-radius: 20px;
  z-index: 2;
}

.content-block {
  display: flex;
  flex-direction: column;
  background-color: #6253FF;
  width: 100%;
  height: 20vh;
  margin: auto 0;
  margin-left: 12px;
}
.text-block {
  color: #fff;
  text-align: center;
  margin: auto
}
.right-block {
  margin: 7vh 70px;
  z-index: 2;
}

.img-card {
  display: flex;
  justify-content: center;
  flex-direction: column;
  position: relative;
  /* max-width: 288px;
  max-height: 200px; */
  cursor: pointer;
}
.card-block {
  opacity: 0;
  transition: opacity 0.5s ease-out;;
}
.card-block:hover {
  opacity: 1;
}
.card-top-block {
  position: absolute;
  top: 10px;
  left: 10px;
  height: 130px;
  width: 91.5%;
  
}
.card-bottom-block {
  position: absolute;
  bottom: 14px;
  left: 10px;
  width: 91.5%;
  height: 50px;
  border-radius: 0 0 10px 10px;
  background-color: #6253FF;
  
}

.button-wrapper {
  display: flex;
  justify-content: center;
  margin-top: 30px;
}
.recipes-btn {
  border: 3px solid #6253FF;
  border-radius: 20px;
  width: 550px;
  height: 70px;
  background: transparent;
  font-size: 16px;
  color: #6253FF;
  cursor: pointer;
  transition: all 0.5s ease-out;
  

}

.recipes-btn:hover {
  color: #fff;
  background: #6253FF;
}


.card-text {
  z-index: 3;
  background-color:#6253FF;
  color: #fff;
}
.image {
  max-width: 288px;
  max-height: 200px;
}
.images-wrapper {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
}

.mediumcircle {
  position: absolute;
  width: 150px;
  height: 150px;
  top: 200px;
  right: 40px;
}
.bigcircle {
  position: absolute;
  width: 300px;
  height: 300px;
  bottom: 0px;
  left: 520px;
  
}
.smallcircle {
  position: absolute;
  width: 110px;
  height: 110px;
  top: 50px;
  left: -30px;
}
</style>