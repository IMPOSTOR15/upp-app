<template>
<header>
  <a class="logo" href="/">
    <img class="logoimg" width="97" height="65" src="../assets/logo.png" alt="logo">
  </a>
  <div class="nav-container">
    <nav>
      <ul class="nav__links">
        <li :active="activeElem === elem"
            @activate="activeElem === elem" 
        >
          <a href="#"><router-link to ='/'>Функционал</router-link></a>
        </li>
        <li>
          <a href="#"><router-link to="/">Статьи</router-link></a>
        </li>
        <li>
          <a href="#"><router-link to="/">Справка</router-link></a>
        </li>
        <li>
          <a href="#"><router-link to="/">Команда</router-link></a>
        </li>
      </ul>
    </nav>
  </div>
  <div class="btn-container">
    <router-link class="cta" to="/login">
      <p class="btn-text">Войти</p>
    </router-link>
  </div>
</header>
</template>

<script>
import { useStore } from 'vuex'

export default {
  setup() {
    const store = useStore();
    const elem = null;
    const activeElem = null;

    return {
      store,
      elem,
      activeElem,
      user: store.state.user,
    }
  },
}
</script>

<style scoped>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  position: relative;
  z-index: 1;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
  opacity: 96%;
  height: 65px;
  position: -webkit-sticky;
  position: sticky;
  top: 15px;
  max-width: 79vw;
  margin: 0 auto;
  z-index: 9;
}

.logo {
  display: block;
  cursor: pointer;
  height: 65px;
  width: 97px;
}

.nav-container {
  display: flex;
  margin: 0 56px 0 auto;
  
}

nav {
  background: #fff;
  display: flex;
  align-items: center;
  justify-content: center; 
  border-radius: 10px; 
  height: 58px;
  -webkit-box-shadow: 0px 5px 24px -4px rgba(65, 0, 90, 0.39);
  -moz-box-shadow: 0px 5px 24px -4px rgba(65, 0, 90, 0.39);
  box-shadow: 0px 5px 24px -4px rgba(65, 0, 90, 0.39);
}


.nav__links a,
.cta,
.overlay__content a {
  font-family: "Montserrat", sans-serif;
  font-weight: 500;
  color: #000000;
  text-decoration: none;
}

.nav__links {
  list-style: none;
  display: flex;
}

.nav__links li {
  width: 11vw;
  padding: 0px 20px;
}

.nav__links li a {
  transition: color 0.3s ease 0s;
}

.nav__links li a:hover {
  color: #6253FF;
}


nav a.router-link-exact-active {
  border-bottom: 2.5px solid #6253FF;
  padding-bottom: 3px;
}

.cta {
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 5px;
  cursor: pointer;
  width: 200px;
  height: 56px;
  transition: background-color 0.3s ease 0s;
  color: #edf0f1;
  background-color: #6253FF;
}

.btn-text {
  color: #fff;
  font-size: 19px;
  text-align: center;
}

.account-btn {
  margin-left: -240px;
  margin-right: 20px;
}

</style>