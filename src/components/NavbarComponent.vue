<template>
<header>
  <a class="logo" href="/"><img class="logoimg" src="../assets/logo.png" alt="logo"></a>
  <nav>
    <ul class="nav__links">
      <li :active="activeElem === elem"
          @activate="activeElem === elem" 
      >
        <a href="#"><router-link to ='/'>Главная</router-link></a>
      </li>
      <li>
        <a href="#"><router-link to="/about">О нас</router-link></a>
      </li>
    </ul>
  </nav>
    <div class="btn-container">
      <router-link class="cta" to="/login">Войти</router-link>
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
  padding: 30px 10%;
  background-color: #27272c;
  opacity: 96%;
  height: 70px;
  position: -webkit-sticky;
  position: sticky;
  top: 0;

}

.logo {
  cursor: pointer;
  width: 40px;
}

.logoimg {
  width: 50px;
}

.nav__links a,
.cta,
.overlay__content a {
  font-family: "Montserrat", sans-serif;
  font-weight: 500;
  color: #ffffff;
  text-decoration: none;
}

.nav__links {
  list-style: none;
  display: flex;
}

.nav__links li {
  padding: 0px 20px;
}

.nav__links li a {
  transition: color 0.3s ease 0s;
}

.nav__links li a:hover {
  color: #27ac3d;
}

nav a.router-link-exact-active {
  border-bottom: 2.5px solid #27ac3d;
  padding-bottom: 3px;
}

.cta {
  padding: 5px 30px;
  background-color: rgb(23, 22, 22);
  border: 2px solid #27ac3d;
  border-radius: 50px;
  cursor: pointer;
  transition: background-color 0.3s ease 0s;
  color: #edf0f1;
  
}

.cta:hover {
  background: #27ac3d;
}
.btn-container {
  display: flex;
  align-items: center;
}
.account-btn {
  margin-left: -240px;
  margin-right: 20px;
}

</style>