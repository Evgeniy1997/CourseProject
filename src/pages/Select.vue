<template>
<form style="width: 376px; margin: 93px 0 0 35px">
  <label class="label__select">Факультет:</label>
  <q-select
    v-model="select"
    :options="selectFacultyOptions"
  />
  <label class="label__select">Курс:</label>
  <q-select
    v-model="select"
    :options="selectCourseOptions"
  />
  <label class="label__select">Специальность:</label>
  <q-select
    v-model="select"
    :options="selectSpecialtyOptions"
  />
  <label class="label__select">Группа:</label>
  <q-select
    v-model="select"
    :options="selectGroupOptions"
  />
  <q-btn class="but" label="Показать" />
</form>
</template>

<style>
  .q-if-standard {
    width: 376px;
    height: 30px;
    border: 1px solid rgba(5,35,143,50%);
    border-radius: 5px;
    color: #05238F !important;
    margin-bottom: 27px;
    padding: 0 0 0 10px !important;
  }

  .q-if-label {
    font-size: 14px;
    color: #05238F !important;
    position: static !important;
    display: flex;
    align-items: center;
  }

  .q-if-label-above {
    margin-bottom: 10px;
  }

  .q-input-target:before {
    content: '' !important;
    color: #05238F !important;
  }

  .q-if-control {
    width: 17px;
    height: 17px;
    border: 1px solid rgba(5,35,143,50%);
    border-radius: 50%;
    color: rgba(5,35,143,50%);
    margin-right: 10px;
  }

  .but {
    width: 100%;
    height: 52px;
    background-color: #0072A9 !important;
    border-radius: 10px;
    color: #fff;
    font-size: 16px;
  }

  .label__select {
    font-size: 16px;
    color: #05238f;
    display: block;
    margin-bottom: 13px;
  }
</style>

<script>
export default {
  name: 'Select',
  data () {
    return {
      selectFacultyOptions: [
        {
          label: 'Биологический',
          value: 'bio'
        },
        {
          label: 'Геолого-географический факультет',
          value: 'geo'
        },
        {
          label: 'Исторический факультет',
          value: 'his'
        },
        {
          label: 'Факультет иностранных языков',
          value: 'for'
        },
        {
          label: 'Факультет матем. и технологий программ.',
          value: 'mat'
        },
        {
          label: 'Факультет психологии и педагогики',
          value: 'psy'
        },
        {
          label: 'Факультет физики и информ. техн.',
          value: 'phy'
        },
        {
          label: 'Факультет физической культуры',
          value: 'cul'
        },
        {
          label: 'Филологический факультет',
          value: 'phi'
        },
        {
          label: 'Экономический факультет',
          value: 'eco'
        },
        {
          label: 'Юридический факультет',
          value: 'law'
        }
      ],
      selectCourseOptions: [
        {
          label: '1',
          value: 'first'
        },
        {
          label: '2',
          value: 'second'
        },
        {
          label: '3',
          value: 'third'
        },
        {
          label: '4',
          value: 'fourth'
        },
        {
          label: '5',
          value: 'fifth'
        }
      ],
      selectSpecialtyOptions: [
        {
          label: '1',
          value: 'first'
        },
        {
          label: '2',
          value: 'second'
        },
        {
          label: '3',
          value: 'third'
        },
        {
          label: '4',
          value: 'fourth'
        },
        {
          label: '5',
          value: 'fifth'
        }
      ],
      selectGroupOptions: [
        {
          label: '1',
          value: 'first'
        },
        {
          label: '2',
          value: 'second'
        },
        {
          label: '3',
          value: 'third'
        },
        {
          label: '4',
          value: 'fourth'
        },
        {
          label: '5',
          value: 'fifth'
        }
      ]
    }
  }
}
</script>
