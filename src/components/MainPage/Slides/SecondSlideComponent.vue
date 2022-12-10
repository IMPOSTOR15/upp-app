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
          <img src="" alt="">
          <p>Фрукты</p>
        </div>
        <div class="img-card">
          <img src="" alt="">
          <p>Рыба</p>
        </div>
        <div class="img-card">
          <img src="" alt="">
          <p>Орехи</p>
        </div>
        <div class="img-card">
          <img src="" alt="">
          <p>Яйца и молочные</p>
        </div>
        <div class="img-card">
          <img src="" alt="">
          <p>Мясо птицы</p>
        </div>
        <div class="img-card">
          <img src="" alt="">
          <p>Полезные завтраки</p>
        </div>
      </div>
      <div class="button-wrapper">
        <button>Смотреть рецепты</button>
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
  background-color: #fff;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  height: 100vh;
}
.left-block {
  display: flex;
  justify-content: center;
  background: #fff url(@/assets/mainPageImages/secondSlide/productsblockbg.png);
  margin: 7vh 0;
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
</style>