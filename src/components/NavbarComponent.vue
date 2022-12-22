<template>
<header>

  <div class="nav-container">

    <a class="logo" href="/">
      <img class="logoimg" src="../assets/logo.png" alt="logo">
    </a>

    <input id="menu__toggle" type="checkbox" />
      <label class="menu__btn" for="menu__toggle">
        <span></span>
      </label>

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

    <div class="btn-container">
      <router-link class="cta" to="/login">
        <p class="btn-text">Войти</p>
      </router-link>
    </div>
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
  
  align-items: center;
  /* padding: 30px 10%; */
  /* background-color: #27272c; */

  opacity: 96%;
  position: -webkit-sticky;
  position: sticky;
  top: 0;
  max-width: 79vw;
  margin: 0 auto;
}

input,.menu__btn,span{
  display: none;
}

.logo {

  justify-self: start;


  cursor: pointer;
  height: 65px;
  width: 97px;
}

.nav-container {
  display: grid;
  margin-top: 40px;

  grid-template-columns: 2fr 2fr 1fr;

  align-items: center;
  gap: 60px;
}

nav {
  background: #fff;
  display: flex;
  align-items: center;
  justify-content: center; 
  /* border: 2px solid black; */
  border-radius: 10px; 
  height: 58px;
  -webkit-box-shadow: 0px 5px 24px -4px rgba(65, 0, 90, 0.39);
  -moz-box-shadow: 0px 5px 24px -4px rgba(65, 0, 90, 0.39);
  box-shadow: 0px 5px 24px -4px rgba(65, 0, 90, 0.39);
}


.nav__links a,
.cta, .overlay__content a {
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
}

/* .nav__links li a {
  transition: color 0.3s ease 0s;
} */

.nav__links li a:hover {
  color: #6253FF;

  border-bottom: 2.5px solid #6153ff2d;
  padding-bottom: 3px;
  transition: padding-bottom .08s;
}


/* Странная штука */
/* nav a.router-link-exact-active {
  border-bottom: 2.5px solid #6253FF;
  padding-bottom: 3px;
} */

.btn-container{
  justify-self: end;
}

.cta {
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 5px;
  cursor: pointer;
  width: 200px;
  height: 56px;
  /* transition: background-color 0.3s ease 0s; */
  color: #edf0f1;
  background-color: #6253FF;
}

/* .btn-text {
  color: #fff;
  font-size: 19px;
  text-align: center;
} */

/* странная штука */
/* .account-btn {
  margin-left: -240px;
  margin-right: 20px;
} */

@media (max-width: 1200px) {
  .nav-container {
    grid-template-columns: 1fr 3fr 1fr;

  }

  .cta{
    width: 100px;
  }
}

@media (max-width: 980px) {
  .btn-container {
    display: none;
  }

  .nav-container {
    width: 100%;
    grid-template-columns: 1fr 1fr;
    justify-content: space-between;

  }

  .menu__btn{
    display: block;
  }

  #menu__toggle {
  opacity: 0;
  }
  #menu__toggle:checked + .menu__btn > span {
    transform: rotate(45deg);
  }
  #menu__toggle:checked + .menu__btn > span::before {
    top: 0px;
    transform: rotate(0deg);
  }
  #menu__toggle:checked + .menu__btn > span::after {
    top: 0px;
    transform: rotate(90deg);
  }
  #menu__toggle:checked ~ .nav__links {
  right: 0 !important;
}

  .menu__btn {
    align-self: center;
    justify-self: end;

    width: 28px;
    height: 28px;
    
    cursor: pointer;
    z-index: 1;
  }
  .menu__btn > span,
  .menu__btn > span::before,
  .menu__btn > span::after {
    display: block;
    position: absolute;

    top: 16px;
    width: 100%;
    height: 2px;
    background-color: #6253FF;
    transition-duration: .25s;
  }
  .menu__btn > span::before {
    content: '';
    top: -8px;
  }
  .menu__btn > span::after {
    content: '';
    top: 8px;
  }

  .nav__links {
    display: block;
    align-self: center;
    justify-self: end;

    

    padding: 80px 0;



    transition-duration: .25s;
  }
  .nav__links a {
    display: block;
    padding: 12px 24px;
    color: #333;
    font-size: 20px;
    text-decoration: none;
    transition-duration: .25s;
  }
}


</style>