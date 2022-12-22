<template>
  <footer class="footer">
    <div class="footer-wrapper">
      <img class="footer-logo" src="@/assets/footerLogo.png" alt="">
      <div class="footer-column">
        <h4 class="column-toplink">Меню</h4>
        <p class="column-link">Функционал</p>
        <p class="column-link">Статьи</p>
      </div>
      <div class="footer-column">
        <h4 class="column-toplink">Прочее</h4>
        <p class="column-link">Политика конфиденциалньости</p>
        <p class="column-link">Информация о команде</p>
      </div>
      <div class="footer-column">
        <h4 class="column-toplink">Помощь</h4>
        <p class="column-link">Служба поддержки</p>
        <p class="column-link">Справка</p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style scoped>
.footer {
  width: 100%;
  height: 130px;
  background-color: #6253FF;
}
.footer-logo {
  widows: 97px;
  height: 65px;
  margin: auto 0;
  cursor: pointer;
}
.footer-wrapper {
  height: 130px;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  margin: 0 170px;
}
.footer-column {
  display: flex;
  flex-direction: column;
  color: #fff;
  text-align: left;
  margin-top: 20px;
}
.column-toplink {
  font-size: 14px;
  margin: 5px 5px;
  cursor: pointer;
}
.column-link {
  font-size: 14px;
  margin: 7px 7px;
  font-weight: lighter;
  cursor: pointer;
}
</style>