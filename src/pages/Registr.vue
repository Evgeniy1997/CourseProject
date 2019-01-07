<template>
 <div id="auth__wrap" style="display:block; width: 100%">
    <p class="link__back" v-on:click="main"><i class="fas fa-external-link-alt"></i>Вернуться на главную страницу</p>
    <div class="wrap">
      <h1 class="auth__title"><i class="fas fa-key"></i>Вход в панель управления</h1>
      <p class="auth__text">Введите существующий логин и пароль для доступа к панели управления</p>
      <div class="form__wrap">
        <form class="auth__form">
          <div class="block__title">
            <h2 class="title">Личные данные</h2>
          </div>
          <label class="label__input" for="firstName">Имя:</label>
          <input type="text" name="firstName" class="input__text" id="firstName">
          <label class="label__input" for="SecondName">Фамилия:</label>
          <input type="text" name="SecondName" class="input__text" id="SecondName">
          <label class="label__input" for="patronymic">Отчество:</label>
          <input type="text" name="Patronymic" class="input__text" id="patronymic">
        </form>
        <form class="auth__form">
          <div class="block__title violet">
            <h2 class="title">Данные университета</h2>
          </div>
          <label class="label__input">Факультет:</label>
          <select class="input__text" id="select">
            <option value="bio" class="option__select">Биологический</option>
            <option value="geo" class="option__select">Геолого-географический факультет</option>
            <option value="his" class="option__select">Исторический факультет</option>
            <option value="lan" class="option__select">Факультет иностранных языков</option>
            <option value="mat" class="option__select">Факультет матем. и технологий программ.</option>
            <option value="psy" class="option__select">Факультет психологии и педагогики</option>
            <option value="phu" class="option__select">Факультет физики и информ. техн.</option>
            <option value="cul" class="option__select">Факультет физической культуры</option>
            <option value="phi" class="option__select">Филологический факультет</option>
            <option value="eco" class="option__select">Экономический факультет</option>
            <option value="law" class="option__select">Юридический факультет</option>
          </select>
          <label class="label__input">Курс:</label>
          <select class="input__text" id="select">
            <option value="1" class="option__select">1</option>
            <option value="2" class="option__select">2</option>
            <option value="3" class="option__select">3</option>
            <option value="4" class="option__select">4</option>
            <option value="5" class="option__select">5</option>
          </select>
          <label class="label__input">Группа:</label>
          <select class="input__text" id="select">
            <option value="ms" class="option__select">МС-42</option>
            <option value="ms" class="option__select">АС-46</option>
            <option value="ms" class="option__select">АС-47</option>
            <option value="ms" class="option__select">СБ-45</option>
            <option value="ms" class="option__select">Ф-43</option>
          </select>
        </form>
        <form class="auth__form">
          <div class="block__title dark-violet">
            <h2 class="title">Данные для авторизации</h2>
          </div>
          <label class="label__input" for="login">Введите логин:</label>
          <input type="text" name="login" class="input__text" id="login">
          <label class="label__input" for="password">Введите пароль:</label>
          <input type="password" name="password" class="input__text" id="password">
          <label class="label__input" for="repeatPassword">Повторите пароль:</label>
          <input type="password" name="password" class="input__text" id="repeatPassword">
        </form>
      </div>
    </div>
    <p class="link__go" v-on:click="auth"><i class="fas fa-external-link-alt"></i>Авторизация</p>
    <q-btn class="but" label="Зарегистрироваться" />
  </div>
</template>

<style scoped>
.violet {
  background: #9966CB !important;
}

.dark-violet {
  background: #4B0081 !important;
}

.option__select {
  height: 31px;
  padding-left: 7px;
  color: #05238F;
  font-size: 12px;
  outline: none;
}

.form__wrap {
  display: flex;
  margin-bottom: 20px;
}

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
  margin: 9px 0px 15px 29px;
}

.but__auth {
  width: 272px;
  height: 41px;
  background-color: #0072A9 !important;
  border-radius: 10px;
  color: #fff;
  font-size: 16px;
  display: block;
  margin: 0px auto;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.05);
}
.but {
    width: 318px;
    height: 52px;
    display: block;
    margin: 0px auto;
    background-color: #0072A9 !important;
    border-radius: 10px;
    color: #fff;
    font-size: 14px;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.05);
  }
</style>

<script>
export default {
  name: 'Registr',
  data () {
    return {
    }
  },
  methods: {
    main: function () {
      var elem1 = document.getElementById('SelectOption')
      var elem2 = document.getElementById('TableList')
      var elem3 = document.getElementById('Registr')
      elem1.style.display = 'block'
      elem2.style.display = 'block'
      elem3.style.display = 'none'
    },
    auth: function () {
      var elem1 = document.getElementById('Auth')
      var elem2 = document.getElementById('Registr')
      elem2.style.display = 'none'
      elem1.style.display = 'block'
    }
  }
}
</script>
