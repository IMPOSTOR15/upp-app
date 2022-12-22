<template>
  <div class="main-wrapper">
    <h2>Статьи</h2>
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
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.main-wrapper {
  margin-top: 300px;
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
  margin: 20px 20px;
}
.article-text{
  margin: 0 20px 20px 20px;
  display: -webkit-box;
  -webkit-line-clamp: 5;
  -webkit-box-orient: vertical;
  overflow: hidden;
}
</style>