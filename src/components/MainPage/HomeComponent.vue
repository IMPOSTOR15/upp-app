<template>
  <div class="main-container">
    <div class="header-container">
      <h1>Мы поможем вам cделать себя лучше</h1>
      <div class="paragraph-container">
        <p class="text20 text-bold">Сайт предоставляет:</p>
        <p class="text20">График питания втечение дня</p>
        <p class="text20">Упражнения для каждой группы мышц</p>
        <p class="text20">Полезные продукты питания</p>
      </div>
      <button class="header-btn">
        <p class="btn-text">Измениться к лучшему</p>
      </button>
    </div>
    <div class="svg-container">
      <img src="@/assets/mainPageImages/mainphoto.svg" alt="">
    </div>
  </div>
  <FirstSlideComponent/>
  <SecondSlideComponent/>
  
</template>

<script>
import FirstSlideComponent from '@/components/MainPage/Slides/FirstSlideComponent.vue'
import SecondSlideComponent from '@/components/MainPage/Slides/SecondSlideComponent.vue'
export default {
  components: {
    FirstSlideComponent,
    SecondSlideComponent
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.main-container {
  display: flex;
  flex-direction: row;
  margin: 70px auto 0 auto;
  max-width: 79vw;
  height: 90vh;
  max-height: 90vh;
}

h1 {
  font-size: 80px;
  text-align: left;
  font-family: 'Exo 2', sans-serif;
}
.header-container {
  margin-right: 8%;
}

.paragraph-container {
  border-left: 3px solid #6253FF;
  padding: 10px 0;
  margin: 0;
  text-align: left;
}

.svg-container {
  max-width: 666;
}

.text-bold {
  font-weight: bold;
}

.text20 {
  font-size: 20px;
  margin: 4px 0 4px 20px;
  font-family: 'Exo 2', sans-serif;
}

.header-btn {
  margin-top: 42px;
  border: none;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 5px;
  cursor: pointer;
  width: 320px;
  height: 80px;
  color: #edf0f1;
  background-color: #6253FF;
}

.btn-text {
  font-size: 20px;
  font-family: 'Exo 2', sans-serif;
}
</style>
