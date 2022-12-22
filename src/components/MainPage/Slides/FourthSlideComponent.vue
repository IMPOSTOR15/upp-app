<template>
  <div class="main-wrapper">
    <h2 class="header-text">Статьи</h2>
    <div class="cards-block">
      <div class="card">
        <div class="arrow">
          <img src="@/assets/mainPageImages/fourthSlide/arrow.svg" alt="">
        </div>
        <div class="img-wrapper">
          <img src="" alt="">
        </div>
        <h4 class="article-header">Lorem ipsum dolor</h4>
        <p class="article-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Consectetur enim ducimus eum deleniti, sapiente cum beatae blanditiis, et, recusandae in distinctio? Ab omnis sed ipsam laborum eius unde illum, neque ipsum sunt voluptas minima suscipit facere, animi, possimus quaerat maxime.</p>
      </div>
      <div class="card">
        <div class="arrow">
          <img src="@/assets/mainPageImages/fourthSlide/arrow.svg" alt="">
        </div>
        <div class="img-wrapper">
          <img src="" alt="">
        </div>
        <h4 class="article-header">Lorem ipsum dolor</h4>
        <p class="article-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Consectetur enim ducimus eum deleniti, sapiente cum beatae blanditiis, et, recusandae in distinctio? Ab omnis sed ipsam laborum eius unde illum, neque ipsum sunt voluptas minima suscipit facere, animi, possimus quaerat maxime.</p>
      </div>
      <div class="card">
        <div class="arrow">
          <img src="@/assets/mainPageImages/fourthSlide/arrow.svg" alt="">
        </div>
        <div class="img-wrapper">
          <img src="" alt="">
        </div>
        <h4 class="article-header">Lorem ipsum dolor</h4>
        <p class="article-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Consectetur enim ducimus eum deleniti, sapiente cum beatae blanditiis, et, recusandae in distinctio? Ab omnis sed ipsam laborum eius unde illum, neque ipsum sunt voluptas minima suscipit facere, animi, possimus quaerat maxime.</p>
      </div>
      <div class="card">
        <div class="arrow">
          <img src="@/assets/mainPageImages/fourthSlide/arrow.svg" alt="">
        </div>
        <div class="img-wrapper">
          <img src="" alt="">
        </div>
        <h4 class="article-header">Lorem ipsum dolor</h4>
        <p class="article-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Consectetur enim ducimus eum deleniti, sapiente cum beatae blanditiis, et, recusandae in distinctio? Ab omnis sed ipsam laborum eius unde illum, neque ipsum sunt voluptas minima suscipit facere, animi, possimus quaerat maxime.</p>
      </div>
      <div class="card">
        <div class="arrow">
          <img src="@/assets/mainPageImages/fourthSlide/arrow.svg" alt="">
        </div>
        <div class="img-wrapper">
          <img src="" alt="">
        </div>
        <h4 class="article-header">Lorem ipsum dolor</h4>
        <p class="article-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Consectetur enim ducimus eum deleniti, sapiente cum beatae blanditiis, et, recusandae in distinctio? Ab omnis sed ipsam laborum eius unde illum, neque ipsum sunt voluptas minima suscipit facere, animi, possimus quaerat maxime.</p>
      </div>
      <div class="card">
        <div class="arrow">
          <img src="@/assets/mainPageImages/fourthSlide/arrow.svg" alt="">
        </div>
        <div class="img-wrapper">
          <img src="" alt="">
        </div>
        <h4 class="article-header">Lorem ipsum dolor</h4>
        <p class="article-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Consectetur enim ducimus eum deleniti, sapiente cum beatae blanditiis, et, recusandae in distinctio? Ab omnis sed ipsam laborum eius unde illum, neque ipsum sunt voluptas minima suscipit facere, animi, possimus quaerat maxime.</p>
      </div>
      <div class="card">
        <div class="arrow">
          <img src="@/assets/mainPageImages/fourthSlide/arrow.svg" alt="">
        </div>
        <div class="img-wrapper">
          <img src="" alt="">
        </div>
        <h4 class="article-header">Lorem ipsum dolor</h4>
        <p class="article-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Consectetur enim ducimus eum deleniti, sapiente cum beatae blanditiis, et, recusandae in distinctio? Ab omnis sed ipsam laborum eius unde illum, neque ipsum sunt voluptas minima suscipit facere, animi, possimus quaerat maxime.</p>
      </div>
      <div class="card">
        <div class="arrow">
          <img src="@/assets/mainPageImages/fourthSlide/arrow.svg" alt="">
        </div>
        <div class="img-wrapper">
          <img src="" alt="">
        </div>
        <h4 class="article-header">Lorem ipsum dolor</h4>
        <p class="article-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Consectetur enim ducimus eum deleniti, sapiente cum beatae blanditiis, et, recusandae in distinctio? Ab omnis sed ipsam laborum eius unde illum, neque ipsum sunt voluptas minima suscipit facere, animi, possimus quaerat maxime.</p>
      </div>
    </div>
    <div class="btn-wrapper">
      <button class="more-btn">Показать ещё</button>
    </div>
    <img class="left-circle" src="@/assets/mainPageImages/fourthSlide/leftcircle.svg" alt="">
    <img class="right-circle" src="@/assets/mainPageImages/fourthSlide/rightcircle.svg" alt="">
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.main-wrapper {
  position: relative;
  margin-top: 300px;
}
.header-text {
  font-size: 32px;
  font-weight: bold;
}
.cards-block {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: space-between;
  margin: 0 10vw;
}
.card {
  display: flex;
  flex-direction: column;
  position: relative;
  width: 335px;
  height: 320px;
  text-align: left;
  border-radius: 20px;
  cursor: pointer;
  margin: 20px 0;
  -webkit-box-shadow: 0px 0px 8px 4px rgba(195, 195, 195, 0.38);
  -moz-box-shadow: 0px 0px 8px 4px rgba(195, 195, 195, 0.38);
  box-shadow: 0px 0px 8px 4px rgba(195, 195, 195, 0.38);
  transition: all 0.5s ease-out;;
}
.card:hover {
  -webkit-box-shadow: 0px 0px 10px 7px rgba(98, 83, 255, 0.5);
  -moz-box-shadow: 0px 0px 10px 7px rgba(98, 83, 255, 0.5);
  box-shadow: 0px 0px 10px 7px rgba(98, 83, 255, 0.5);
}
.arrow {
  position: absolute;
  right: 20px;
  top: 20px;
}
.img-wrapper {
  width: 100%;
  min-height: 137px;
  background: #c9c4ff;
  border-radius: 20px 20px 0 0;
}
.article-header {
  margin: 15px 20px;
  font-size: 20px;
  font-weight: bold;
}
.article-text{
  margin: 0 20px 20px 20px;
  display: -webkit-box;
  -webkit-line-clamp: 5;
  -webkit-box-orient: vertical;
  overflow: hidden;
  font-size: 16px;
}
.btn-wrapper {
  margin: 40px 0;
}

.more-btn {
  height: 60px;
  width: 300px;
  background-color: transparent;
  color: #6253FF;
  border: 2px solid #6253FF;
  border-radius: 10px;
  cursor: pointer;
  font-size: 20px;
  transition: 0.3s all ease-in-out;
}

.more-btn:hover {
  background-color: #6253FF;
  color: #fff;
  -webkit-box-shadow: 0px 0px 10px 7px rgba(98, 83, 255, 0.5);
  -moz-box-shadow: 0px 0px 10px 7px rgba(98, 83, 255, 0.5);
  box-shadow: 0px 0px 10px 7px rgba(98, 83, 255, 0.5);
}

.left-circle {
  position: absolute;
  left: 0px;
  top: 60%;
  overflow: hidden;
}
.right-circle {
  position: absolute;
  right: 0px;
  top: 10%;
  overflow: hidden;
}
</style>