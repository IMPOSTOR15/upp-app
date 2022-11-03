<template>
  <h1>Войдите в аккаунт</h1>
  <div class="login">
    <form class="login" @submit.prevent = "login">
      <input
        type="email"
        placeholder="Адрес Email" />
      <input type="password"
        placeholder="Пароль" />
      <input
        type="submit"
        value="Войти" />
    </form>
    <router-link class="button" to="/rememberpassword">Забыли пароль?</router-link>
    <router-link class="button" to="/registration">Зарегистрироваться</router-link>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>