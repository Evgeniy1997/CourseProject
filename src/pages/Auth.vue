<template>
  <div id="auth__wrap" style="display:block; width: 100%">
    <p class="link__back" v-on:click="main"><i class="fas fa-external-link-alt"></i>Вернуться на главную страницу</p>
    <div class="wrap">
      <h1 class="auth__title"><i class="fas fa-key"></i>Вход в панель управления</h1>
      <p class="auth__text">Введите существующий логин и пароль для доступа к панели управления</p>
      <form class="auth__form">
        <div class="block__title">
          <h2 class="title">Авторизация</h2>
        </div>
        <label class="label__input">Введите логин:</label>
        <input type="text" name="login" class="input__text">
        <label class="label__input">Введите пароль:</label>
        <input type="password" name="password" class="input__text">
        <q-btn class="but__auth" label="Войти" />
      </form>
    </div>
    <p class="link__go" v-on:click="registr"><i class="fas fa-external-link-alt"></i>Регитрация</p>
  </div>
</template>

<style scoped>
.link__back {
  position: absolute;
  left: 52px;
  top: 116px;
  font-weight: 300;
  font-size: 12px;
  color: #05238F;
  cursor: pointer;
}

.link__go {
  position: absolute;
  right: 52px;
  top: 116px;
  font-weight: 300;
  font-size: 12px;
  color: #05238F;
  cursor: pointer;
}

.fa-external-link-alt {
  font-size: 10px;
  margin-right: 7px;
}

.auth__form {
  padding-bottom: 30px;
}

.auth__title {
  margin-top: 42px;
  font-size: 20px;
  font-weight: 700;
  text-align: center;
}

.fa-key {
  font-size: 16px;
  margin-right: 7px;
}

.auth__text {
  font-size: 14px;
  font-weight: 200;
  text-align: center;
  margin-top: 29px;
  margin-bottom: 29px;
}

.auth__form {
  border-radius: 10px;
  width: 330px;
  margin: 0px auto;
  box-shadow: 0px 4px 14px rgba(0, 0, 0, 0.07);
}

.block__title {
  display: flex;
  width: 330px;
  height: 62px;
  background: #6601FF;
  box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.15);
  border-radius: 10px 10px 0px 0px;
  align-items: center;
  margin-bottom: 24px;
}

.title {
  margin: 0px auto;
  padding: 0;
  font-size: 16px;
  font-weight: 400;
  color: #FFF;
}

.label__input {
  font-weight: 200;
  font-size: 14px;
  color: #05238F;
  margin-left: 29px;
}

.input__text {
  width: 272px;
  height: 30px;
  border: 1px solid rgba(5, 35, 143, 0.5);
  box-sizing: border-box;
  border-radius: 5px;
  font-weight: 300;
  font-size: 12px;
  color: #05238F;
  outline: none;
  padding-left: 7px;
  margin: 9px 0px 21px 29px;
}

.but__auth {
  width: 272px;
  height: 41px;
  background-color: #0072A9 !important;
  border-radius: 10px;
  color: #fff;
  font-size: 14px;
  display: block;
  margin: 0px auto;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.05);
}
</style>

<script>
export default {
  name: 'Auth',
  data () {
    return {
    }
  },
  methods: {
    main: function () {
      var elem1 = document.getElementById('SelectOption')
      var elem2 = document.getElementById('TableList')
      var elem3 = document.getElementById('Auth')
      elem1.style.display = 'block'
      elem2.style.display = 'block'
      elem3.style.display = 'none'
    },
    registr: function () {
      var elem1 = document.getElementById('Auth')
      var elem2 = document.getElementById('Registr')
      elem1.style.display = 'none'
      elem2.style.display = 'block'
    }
  }
}
</script>
