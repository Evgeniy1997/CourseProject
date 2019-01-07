<template>
  <q-layout>
      <!-- Round shaped (only use icon or spinner as content!) with loading state -->
    <q-toolbar class="toolbar">
      <!--
        For Toolbar title, we use
        QToolbarTitle component
      -->
      <q-toolbar-title class="toolbar__logo">
        <img src="../assets/logo.png" alt="logo" class="logo">
        <h1 class="logo__title">ГОМЕЛЬСКИЙ ГОСУДАРСТВЕННЫЙ<br>
          УНИВЕРСИТЕТ ИМ. Ф. СКОРИНЫ</h1>
      </q-toolbar-title>
      <q-btn label="Панель управления" v-on:click="display" class="toolbar__btn" id="toolbar__btn"/>
    </q-toolbar>

    <div class="wrapper">
      <q-page-container id="SelectOption">
        <SelectOption></SelectOption>
      </q-page-container>
      <q-page-container id="TableList">
        <TableList></TableList>
      </q-page-container>
      <q-page-container id="Auth" style="display: none; width: 100%;">
        <Auth></Auth>
      </q-page-container>
      <q-page-container id="Registr" style="display: none; width: 100%;">
        <Registr></Registr>
      </q-page-container>
    </div>
  </q-layout>
</template>

<script>
import { openURL } from 'quasar'
import TableList from '../pages/Table'
import SelectOption from '../pages/Select'
import Auth from '../pages/Auth'
import Registr from '../pages/Registr'
export default {
  name: 'MyLayout',
  components: {SelectOption, TableList, Auth, Registr},
  data () {
    return {

    }
  },
  methods: {
    display: function () {
      var elem1 = document.getElementById('SelectOption')
      var elem2 = document.getElementById('TableList')
      var elem3 = document.getElementById('Registr')
      var elem4 = document.getElementById('Auth')
      elem1.style.display = 'none'
      elem2.style.display = 'none'
      elem3.style.display = 'none'
      elem4.style.display = 'block'
    },
    openURL
  }
}
</script>

<style scoped>
  .wrapper {
    display: flex;
  }

  .toolbar {
    height: 70px;
    background-color: #23282d !important;
    padding: 0;
    margin: 0;
  }

  .toolbar__logo {
    display: flex;
  }

  .logo {
    width: 53px;
    height: 53px;
    margin-left: 35px;
  }

  .logo__title {
    width: 271px;
    font-size: 16px;
    display: flex;
    align-items: center;
    margin: 0 0 0 24px;
    padding: 0;
  }

   .toolbar__btn {
    height: 70px;
    width: 264px;
    padding: 0;
    margin: 0;
  }
  .toolbar__btn:hover {
    background-color: #0072a9;
  }
</style>
