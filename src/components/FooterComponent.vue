<template>
  <footer class="footer">
    <div class="logo-wrapper">
      <img class="footer-logo" src="@/assets/footerLogo.png" alt="">
    </div>
    <div class="footer-wrapper">
      <div class="footer-column">
        <h4 class="column-toplink">Меню</h4>
        <p class="column-link">&bull; Функционал</p>
        <p class="column-link">&bull; Статьи</p>
      </div>
      <div class="footer-column">
        <h4 class="column-toplink">Прочее</h4>
        <p class="column-link">&bull; Политика конфиденциалньости</p>
        <p class="column-link">&bull; Информация о команде</p>
      </div>
      <div class="footer-column">
        <h4 class="column-toplink">Помощь</h4>
        <p class="column-link">&bull; Служба поддержки</p>
        <p class="column-link">&bull; Справка</p>
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
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}
.logo-wrapper {
  margin: auto 50px;
}
.footer-logo {
  width: 97px;
  height: 65px;
  cursor: pointer;
}
.footer-wrapper {
  width: 1400px;
  /* height: 130px; */
  display: flex;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
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
@media (max-width: 1200px) {
  .footer-wrapper {
    width: 900px;
    justify-content: space-between;
  }
  .footer-column {
    margin: 20px;
  }
}
@media (max-width: 980px) {
  .footer {
    height: auto;
    flex-direction: column;
    justify-content: space-between;
  }
  .footer-logo {
    width: 70px;
    height: 50px;
    margin-top: 10px;
  }
  .footer-wrapper {
    width: 100%;
  }
  .footer-column {
    margin-top: 10px;
    margin: 10px;
  }
  .column-toplink {
    font-size: 12px;
    margin: 5px 0;
    text-align: center;
  }
  .column-link {
    font-size: 9px;
    margin: 7px 0;
  }
}



</style>