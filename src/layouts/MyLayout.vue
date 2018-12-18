<template>
  <q-layout view="lHh Lpr lFf">
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
      <q-btn label="Панель управления" class="toolbar__btn"/>
    </q-toolbar>

    <div class="wrapper">
      <q-page-container>
        <Select></Select>
      </q-page-container>
      <q-page-container>
        <Table></Table>
      </q-page-container>
    </div>
  </q-layout>
</template>

<script>
import { openURL } from 'quasar'
import Table from '../pages/Table'
import Select from '../pages/Select'

export default {
  name: 'MyLayout',
  components: {Select, Table},
  data () {
    return {

    }
  },
  methods: {
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
    text-align: center;
  }

  .toolbar__btn:hover {
    background-color: #0072a9;
  }
</style>
