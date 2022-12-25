<template>
  <div class="main-wrapper">
    <div class="background-color"></div>
    <div class="top-wrapper">
      <div class="top-left-block">
        <h2 class="header-title">Таймер упражнений</h2>
        <p class="text-title">Позволяет легко отслеживать продлжительность упражнений и отдыха, чтобы вы могли сосредоточиться на эффективной треннировке</p>
      </div>
      <div class="top-right-block">
      </div>
    </div>
    <div class="bottom-wrapper">
      <div class="bottom-left-block">
        <h2 class="header-title">Упражнения</h2>
        <p class="text-title">Популярные упражнения для всех групп мыщц, с видео выполненияем</p>
        <div class="bottom-left-placeholder"></div>
      </div>
      <div class="bottom-right-block">
        <h2 class="header-title">Получай достижения</h2>
        <p class="text-title">За прохождение серии тренировок, получай достижения, которые будут показывать ваше достижение в тренировках</p>
        <div class="achivment-row">
          <div class="achivment"></div>
          <div class="achivment"></div>
          <div class="achivment"></div>
        </div>
        <button class="right-button">Начать упражнения</button>
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
  position: relative;
  background-color: transparent;
  display: flex;
  flex-direction: column;
  align-self: center;
  height: 130vh;
  margin-top: 50px;
  margin: 50px auto;
}
.top-wrapper {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  margin: 0 auto;
}

.top-left-block {
  width: 400px;
  text-align: left;
  margin-right: 100px;
}
.header-title {
  font-weight: bold;
  font-size: 24px;
}
.text-title {
  font-size: 20px;
}
.top-right-block {
  min-width: 442px;
  height: 347px;
  background: #6253FF;
  border-radius: 20px;
}

.bottom-wrapper {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  /* width: 50vw; */
  margin: 120px auto 0 auto;
}

.bottom-left-block {
  margin: 80px 20px 0 20px;
  width: 442px;
  text-align: left;
}

.bottom-right-block {
  margin: 0px 20px 0 20px;
  width: 442px;
  text-align: left;
}

.bottom-left-placeholder {
  width: 442px;
  height: 541px;
  background: #6253FF;
  border-radius: 20px;
}

.achivment-row {
  margin-top: 50px;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}

.achivment {
  width: 100px;
  height: 100px;
  background: #6253FF;
  border-radius: 50px;
}
.right-button {
  margin-top: 300px;
  width: 100%;
  height: 60px;
  background: transparent;
  border: 2px #6253FF solid;
  color: #6253FF;
  font-size: 20px;
  border-radius: 10px;
  transition: all 0.5s ease-out;;
  cursor: pointer;
}

.right-button:hover {
  background: #6253FF;
  color: #fff;
}
.background-color {
  position: absolute;
  top: 233px;
  width: 100%;
  height: 100%;
  opacity: 0.5;
  background-color: #6253FF;
  z-index: -1;
  overflow:hidden;
}


@media (max-width: 1200px) {
  
}
@media (max-width: 980px) {
  .main-wrapper {
    
    height: auto;
  }
  .top-wrapper {
    flex-direction: column;
    display: flex;
    justify-content: center;
    flex-direction: column;
    width: 80vw;
  }
  .top-left-block {
    width: 80vw;
  }
  .top-right-block {
    min-width: 80vw;
  }
  .bottom-wrapper {
    width: 80vw;
    flex-direction: column;
    margin: 0 auto 0 auto;
  }
  .bottom-left-block {
    display: flex;
    justify-content: center;
    flex-direction: column;
    margin: 30px 0 0 0;
    width: 100%;
    text-align: left;
  }
  .bottom-right-block {
    width: 100%;
  }
  .bottom-right-block {
    display: flex;
    justify-content: center;
    flex-direction: column;
    margin: 30px 0 0 0;
    width: 100%;
    text-align: left;
  }
  .bottom-left-placeholder {
    width: 100%;
  }
  .right-button {
    margin-top: 50px;
  }
  .background-color {
    height: 90%;
  }
}  
</style>