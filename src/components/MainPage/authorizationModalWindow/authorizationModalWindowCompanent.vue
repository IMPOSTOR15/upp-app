<template>
  <transition name="modal">
    <div v-if="show" class="modal-shadow" @click.self="closeModal">
      <div class="modal">
        <div class="modal-close" @click="closeModal">&#10006;</div>
        <slot name="body">
          <div class="container">
            <div class="frame" :class="{'frame-long' : isRegistration}">
              <div class="nav">
                <ul class = "links">
                  <li :class="{ 'signin-active' : isLogin , 'signin-inactive' : isRegistration }" ><a class="btn" @click="changeToLogin">Вход</a></li>
                  <li :class="{ 'signup-inactive' : isLogin, 'signup-active' : isRegistration}" ><a class="btn" @click="changeToRegistration">Регистрация</a></li>
                </ul>
              </div>
              <form class="form-signin" :class="{'form-signin-left' : isRegistration}" name="form">
                <label for="username" >Имя пользователя</label>
                <input class="form-styling" type="text" name="username" placeholder=""/>
                <label for="password">Пароль</label>
                <input class="form-styling" type="password" name="password" placeholder=""/>
                <input type="checkbox" id="checkbox"/>
                <label for="checkbox" >
                  <span class="ui"></span>
                  Оставаться в системе
                </label>
                <div class="btn-animate">
                  <a class="btn-signin">Войти</a>
                </div>
              </form>
              <form class="form-signup" :class="{ 'form-signup-left' : isRegistration}" name="form">
                <label for="fullname">Полное имя</label>
                <input class="form-styling" type="text" name="fullname" placeholder=""/>
                <label for="email">Электронная почта</label>
                <input class="form-styling" type="text" name="email" placeholder=""/>
                <label for="password">Пароль</label>
                <input class="form-styling" type="password" name="password" placeholder=""/>
                <label for="confirmpassword">Подтвредить пароль</label>
                <input class="form-styling" type="text" name="confirmpassword" placeholder=""/>
                <a class="btn-signup">Зарегистрироваться</a>
              </form>
            </div>
          </div>
        </slot>
      </div>
    </div>
  </transition>
</template>
 
<script>
export default {
  name: "ModalWindow",
  data: function () {
    return {
      show: false,
      isLogin: true,
      isRegistration: false,
    }
  },
  methods: {
    closeModal() {
      this.show = false
    },
    changeToRegistration() {
      this.isRegistration = true;
      this.isLogin = false;
    },
    changeToLogin() {
      this.isRegistration = false;
      this.isLogin = true;
    }
  }
}
</script>
 
<style scoped>
.modal-shadow {
  position: fixed;
  top: 0;
  left: 0;
  min-height: 100%;
  width: 100%;
  background: rgba(0, 0, 0, 0.39);
  z-index: 9;
}

.modal {
  box-sizing: border-box;
  background-size: cover;
  background: #fff;
  border-radius: 8px;
  /* padding: 15px; */
  min-width: 420px;
  max-width: 480px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.modal-enter-active,
.modal-leave-active {
  transition: opacity 0.5s ease
}

.modal-enter-from,
.modal-leave-to {
  opacity: 0
}
.modal-close {
  border-radius: 50%;
  color: #fff;
  background: #6253FF;
  display: flex;
  align-items: center;
  justify-content: center;
  position: absolute;
  top: 7px;
  right: 7px;
  width: 30px;
  height: 30px;
  cursor: pointer;
}

html, body * { box-sizing: border-box; }

.container {
  width: 100%;
}

.frame {
  height: 575px;
  width: 430px;
  background:
    linear-gradient(
    rgba(35,43,85,0.75),
    rgba(35,43,85,0.95));
  background-size: cover;
  margin-left: auto;
  margin-right: auto;
  border-radius: 8px;
  box-shadow: 0px 2px 7px rgba(0,0,0,0.2);
  overflow: hidden;
  transition: all .5s ease;
}

.frame-long {
  height: 615px;
}

.frame-short {
  height: 400px;
  margin-top: 50px;
  box-shadow: 0px 2px 7px rgba(0,0,0,0.1);
}

.nav {
  width: 100%;
  height: 100px;
  padding-top: 30px;
  opacity: 1;
  transition: all .5s ease;
}

.nav-up {
  transform: translateY(-100px);
  opacity: 0;
}

li {
  padding-left: 10px;
  font-size: 18px;
  display: inline;
  text-align: left;
  text-transform: uppercase;
  padding-right: 10px;
  color: #000000;
}

.signin-active a {
  padding-bottom: 10px;
  color: #000000;
  text-decoration: none;
  border-bottom: solid 2px #1059FF;
  transition: all .25s ease;
  cursor: pointer;
}

.signin-inactive a {
  padding-bottom: 0;
  color: rgba(255,255,255,.3);
  text-decoration: none;
  border-bottom: none;
  cursor: pointer;
}

.signup-active a {
  cursor: pointer;
  color: #000000;
  text-decoration: none;
  border-bottom: solid 2px #1059FF;
  padding-bottom: 10px;
}

.signup-inactive a {
  cursor: pointer;
  color: rgba(255,255,255,.3);
  text-decoration: none;
  transition: all .25s ease;
}

.form-signin {
  max-width: 430px;
  height: 375px;
	font-size: 16px;
	font-weight: 300;
  padding-left: 37px;
  padding-right: 37px;
  padding-top: 55px;
  transition: opacity .5s ease, transform .5s ease;
}

.form-signin-left {
  transform: translateX(-400px);
  opacity: 0;
}

.form-signup {
  width: 430px;
  height: 375px;
	font-size: 16px;
	font-weight: 300;
  padding-left: 37px;
  padding-right: 37px;
  padding-top: 25px;
  position: relative;
  top: -375px;
  left: 400px;
  opacity: 0;
  transition: opacity .5s ease, transform .5s ease;
}

.form-signup-left {
  transform: translateX(-400px);
  opacity: 1;
}

.form-signup-down {
  top: 0px;
  opacity: 0;
}

.success {
  width: 80%;
  height: 150px;
  text-align: center;
  position: relative;
  top: -890px;
  left: 450px;
  opacity: .0;
  transition: all .8s .4s ease;
}

.success-left {
  transform: translateX(-406px);
  opacity: 1;
}

.successtext {
  color: #000000;
	font-size: 16px;
	font-weight: 300;
  margin-top: -35px;
  padding-left: 37px;
  padding-right: 37px;
}

#check path {
    stroke: #000000;
    stroke-linecap:round;
    stroke-linejoin:round;
    stroke-width: .85px;
    stroke-dasharray: 60px 300px;
    stroke-dashoffset: -166px;
    fill: rgba(255,255,255,.0);
    transition: stroke-dashoffset 2s ease .5s, fill 1.5s ease 1.0s;
}

#check.checked path {
    stroke-dashoffset: 33px;
    fill: rgba(255,255,255,.03);
}

.form-signin input, .form-signup input {
  color: #000000;
  font-size: 15px;
}

.form-styling {
  width: 100%;
  height: 35px;
	padding-left: 15px;
	border: none;
	border-radius: 20px;
  margin-bottom: 20px;
  background: rgba(255,255,255,.2);
  color: #000000;
  background-color: #6153ff80;
}

label {
  font-weight: 400;
  text-transform: uppercase;
  font-size: 15px;
  padding-bottom: 12px;
  color: #000000;
  display: block;
  text-align: left;
  padding-left: 10px;
}

:focus {outline: none;
}

.form-signin input:focus, textarea:focus, .form-signup input:focus, textarea:focus {
    background: #6153ffc0;
    border: none; 
    padding-right: 40px;
    transition: background .5s ease;
 }

[type="checkbox"]:not(:checked),
[type="checkbox"]:checked {
  position: absolute;
  display: none;
}

[type="checkbox"]:not(:checked) + label,
[type="checkbox"]:checked + label {
  position: relative;
  padding-left: 85px;
  padding-top: 2px;
  cursor: pointer;
  margin-top: 8px;
}

[type="checkbox"]:not(:checked) + label:before,
[type="checkbox"]:checked + label:before,
[type="checkbox"]:not(:checked) + label:after,
[type="checkbox"]:checked + label:after {
  content: '';
  position: absolute;
}

[type="checkbox"]:not(:checked) + label:before,
[type="checkbox"]:checked + label:before {
  width: 65px; 
  height: 30px;
  background: #6153ff80;
  border-radius: 15px;
  left: 0; 
  top: -3px;
  transition: all .2s ease;
}

[type="checkbox"]:not(:checked) + label:after,
[type="checkbox"]:checked + label:after {
  width: 10px; 
  height: 10px;
  background: #fff;
  border-radius: 50%;
  top: 7px; 
  left: 10px;
  transition: all .2s ease;
}

/* on checked */
[type="checkbox"]:checked + label:before {
  background: #6253FF; 
}

[type="checkbox"]:checked + label:after {
  background: #fff;
  top: 7px; 
  left: 45px;
}

[type="checkbox"]:checked + label .ui,
[type="checkbox"]:not(:checked) + label .ui:before,
[type="checkbox"]:checked + label .ui:after {
  position: absolute;
  left: 6px;
  width: 65px;
  border-radius: 15px;
  font-size: 14px;
  font-weight: bold;
  line-height: 22px;
  transition: all .2s ease;
}

[type="checkbox"]:not(:checked) + label .ui:before {
  content: "no";
  left: 32px;
  color: rgba(255,255,255,.7);
}

[type="checkbox"]:checked + label .ui:after {
  content: "yes";
  color: #ffffff;
}

[type="checkbox"]:focus + label:before {
  box-sizing: border-box;
  margin-top: -1px;
}

.checkbox-text {
  margin: 0;
}
.links {
  /* padding: 0; */
  text-align: left;
}
.btn-signup {
  float: left;
  font-weight: 700;
  text-transform: uppercase;
  font-size: 13px;
  text-align: center;
  color: #ffffff;
  padding-top: 8px;
  width: 100%;
  height: 35px;
	border: none;
	border-radius: 20px;
  margin-top: 23px;
  background-color: #1059FF;
}

.btn-signin {
  float: left;
  padding-top: 10px;
  width: 100%;
  height: 35px;
	border: none;
	border-radius: 20px;
  margin-top: -8px;
}

.btn-animate {
  float: left;
  font-weight: 700;
  text-transform: uppercase;
  font-size: 13px;
  text-align: center;
  color: rgba(255,255,255, 1);
  padding-top: 8px;
  width: 100%;
  height: 35px;
	border: none;
	border-radius: 20px;
  margin-top: 23px;
  background-color: #6153ffc0;
  left: 0px;
  top: 0px;
  transition: all .5s ease, top .5s ease .5s, height .5s ease .5s, background-color .5s ease .75s; 
}

.btn-animate-grow {
  width: 130%;
  height: 625px;
  position: relative;
  left: -55px;
  top: -420px;
  color: rgba(255,255,255,0);
  background-color: rgba(255,255,255,1);
}

a.btn-signup:hover, a.btn-signin:hover {
    cursor: pointer; 
    background-color: #6153ff;
    transition: background-color .5s; 
}

.forgot {
  height: 100px;
  width: 80%;
  margin-left: auto;
  margin-right: auto;
  text-align: center;
  padding-top: 24px;
  margin-top: -535px;
  transition: all 0.5s ease;
}

.forgot-left {
  transform: translateX(-400px);
  opacity: 0;
}

.forgot-fade {
  opacity: 0;
}

.forgot a {
  color: rgba(255,255,255,.3);
  font-weight: 400;
  font-size: 13px;
  text-decoration: none;
}

</style>