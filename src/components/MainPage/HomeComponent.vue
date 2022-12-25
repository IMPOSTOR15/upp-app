<template>
  <div class="main-container">


    <div class="header-container">

      <h1>Мы поможем вам cделать себя лучше</h1>

      <div class="paragraph-container">
        <p class="text-bold">Сайт предоставляет:</p>
        <p>График питания втечение дня</p>
        <p>Упражнения для каждой группы мышц</p>
        <p>Полезные продукты питания</p>
      </div>

      <button class="header-btn"> Измениться к лучшему</button>
    </div>

    <div class="svg-container">
      <img src="@/assets/mainPageImages/mainphoto.svg" alt="">
    </div>
  </div>

  <FirstSlideComponent/>
  <SecondSlideComponent/>
  <ThirdSlideComponent/>
  <FouthSlideComponent/>
  
</template>

<script>
import FirstSlideComponent from '@/components/MainPage/Slides/FirstSlideComponent.vue'
import SecondSlideComponent from '@/components/MainPage/Slides/SecondSlideComponent.vue'
import ThirdSlideComponent from '@/components/MainPage/Slides/ThirdSlideComponent.vue'
import FouthSlideComponent from '@/components/MainPage/Slides/FourthSlideComponent.vue'
export default {
  components: {
    FirstSlideComponent,
    SecondSlideComponent,
    ThirdSlideComponent,
    FouthSlideComponent
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.main-container {
  display: flex;
  justify-content: space-between;

  margin: 120px auto 246px auto;
  max-width: 79vw;
}

h1 {
  font-size: 80px;
  text-align: left;
  font-family: 'Exo 2', sans-serif;
  margin-block-end: 0em;
  margin-block-start: 0em;

  transition: 0.3s all ease-out;
}
.header-container {
  display: grid;
}

.paragraph-container {
  height: 160px;
  padding: 10px 0;
  border-left: 3px solid #6253FF;
  text-align: left;
  align-self: end;
}

.paragraph-container p {
  font-size: 20px;
  margin: 10px 0 0px 20px;
  font-family: 'Exo 2', sans-serif;

  transition: 0.3s all ease-out;
}

.svg-container {
  align-self: flex-start;
  width: 100%;
}
.svg-container img {

    transition: 0.3s all ease-out;
    width: 100%;
  }

.text-bold {
  font-weight: bold;
}

.header-btn {
  width: 320px;
  height: 80px;
  border-radius: 5px;
  border: none;

  display: flex;
  align-items: center;
  justify-content: center;
  align-self: flex-end;
  
  cursor: pointer;
  font-size: 20px;
  color: #edf0f1;
  font-family: 'Exo 2', sans-serif;
  background-color: #6253FF;

  transition: 0.3s all ease-out;
}

.header-btn:hover {
  font-size: 22px;
  -webkit-box-shadow: 0px 0px 10px 5px rgba(98, 83, 255, 0.5);
  -moz-box-shadow: 0px 0px 10px 5px rgba(98, 83, 255, 0.5);
  box-shadow: 0px 0px 10px 5px rgba(98, 83, 255, 0.5);
}


@media (max-width: 1680px) {
  h1 {
    font-size: 68px;
  }

  .paragraph-container{
    height: 140px;
    padding: 0px 0;
  }
  .paragraph-container p {
    font-size: 16px;
  }
}

@media (max-width: 1460px) {
  h1 {
    font-size: 48px;
    
  }
  .paragraph-container{
    height: 126px;
  }
  .paragraph-container p {
    font-size: 16px;
  }
}

@media (max-width: 1200px) {
  h1 {
    font-size: 38px;
  }

  .header-btn {
    width: 300px;
    height: 56px;

    font-size: 18px;
  }
  .paragraph-container p {
    font-size: 14px;
  }
}

@media (max-width: 980px) {


  .main-container{
    margin-top: 32px;
    display: grid;
    justify-content: center;
    
  }

  h1 {
    text-align: center;
    
    grid-row-start: 1;

    font-size: 36px;
    margin-bottom: 24px;
  }


  .svg-container{
    grid-row-start: 2;
    position: relative;
  }

  .svg-container img{
    height: 380px;
  }

  .paragraph-container{
    position: absolute;
    top:660px;
  }

  .paragraph-container p {
    font-size: 14px;
  }

  .header-btn {
    position: absolute;

    top:800px;


    width: 320px;
    height: 80px;

    font-size: 18px;
  }

}

</style>
