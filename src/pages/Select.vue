<template>
<form style="width: 376px; margin: 63px 0 0 35px">
  <label class="label__select">Факультет:</label>
  <select class="select" id="select">
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
  <label class="label__select">Курс:</label>
  <select class="select" id="select">
    <option value="1" class="option__select">1</option>
    <option value="2" class="option__select">2</option>
    <option value="3" class="option__select">3</option>
    <option value="4" class="option__select">4</option>
    <option value="5" class="option__select">5</option>
  </select>
  <label class="label__select">Группа:</label>
  <select class="select" id="select">
    <option value="ms" class="option__select">МС-42</option>
    <option value="ms" class="option__select">АС-46</option>
    <option value="ms" class="option__select">АС-47</option>
    <option value="ms" class="option__select">СБ-45</option>
    <option value="ms" class="option__select">Ф-43</option>
  </select>
  <q-btn class="but" label="Показать" />
</form>
</template>

<style>
  .select {
    margin-bottom: 27px;
    width: 376px;
    height: 30px;
    border: 1px solid rgba(5, 35, 143, 0.5);
    border-radius: 5px;
    color: #05238F;
    font-size: 12px;
    font-weight: 200;
    padding-left: 7px;
    outline: none;
  }

  .option__select {
    height: 31px;
    padding-left: 7px;
    color: #05238F;
    font-size: 12px;
    outline: none;
  }

  .label__select {
    font-size: 16px;
    color: #05238f;
    display: block;
    margin-bottom: 13px;
  }
  .but {
    width: 100%;
    height: 52px;
    background-color: #0072A9 !important;
    border-radius: 10px;
    color: #fff;
    font-size: 16px;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.05);
  }
</style>

<script>
export default {
  name: 'Select',
  data () {
    return {
    }
  }
}
</script>
