<template>
  <div class="main-wrapper">
    <div class="left-block">
      <!-- <img class="bg-img" src="@/assets/mainPageImages/secondSlide/productsblockbg.png" alt=""> -->
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
          <img src="@/assets/mainPageImages/secondSlide/cards/first.png" alt="">
          <p>Фрукты</p>
        </div>
        <div class="img-card">
          <img src="@/assets/mainPageImages/secondSlide/cards/second.png" alt="">
          <p>Рыба</p>
        </div>
        <div class="img-card">
          <img src="@/assets/mainPageImages/secondSlide/cards/third.png" alt="">
          <p>Орехи</p>
        </div>
        <div class="img-card">
          <img src="@/assets/mainPageImages/secondSlide/cards/fourth.png" alt="">
          <p>Яйца и молочные</p>
        </div>
        <div class="img-card">
          <img src="@/assets/mainPageImages/secondSlide/cards/fifth.png" alt="">
          <p>Мясо птицы</p>
        </div>
        <div class="img-card">
          <img src="@/assets/mainPageImages/secondSlide/cards/sixth.png" alt="">
          <p>Полезные завтраки</p>
        </div>
      </div>
      <div class="button-wrapper">
        <button>Смотреть рецепты</button>
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
  background: #fff url(@/assets/mainPageImages/secondSlide/productsblockbg.png);
  margin: 7vh 0;
  z-index: 2;
}

.content-block {
  display: flex;
  flex-direction: column;
  background-color: #6253FF;
  width: 40vw;
  height: 20vh;
  margin: auto 0;
}
.text-block {
  color: #fff;
  text-align: center;
  margin: auto
}
.right-block {
  margin: 7vh 30px;
  z-index: 2;
}
.images-wrapper {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
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