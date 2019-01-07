<template>
<div>
  <q-table
    title="Расписание для группы МС-42"
    :data="tableData"
    :columns="columns"
    row-key="name"
  />
</div>
</template>

<style>
  .q-table-container {
    margin: 56px 0px 0px 20px;
    width: 920px;
  }

  .q-table td {
    white-space: normal !important;
    padding: 5px 10px !important;
  }
</style>

<script>

export default {
  name: 'TableList',
  data: () => ({
    columns: [
      {
        name: 'time',
        required: true,
        label: 'Время',
        align: 'center',
        field: 'time',
        sortable: true,
        classes: 'my-class'
      },
      {
        name: 'monday',
        required: true,
        label: 'Понедельник',
        align: 'center',
        field: 'monday',
        sortable: true,
        classes: 'my-class'
      },
      {
        name: 'tuesday',
        required: true,
        label: 'Вторник',
        align: 'center',
        field: 'tuesday',
        sortable: true,
        classes: 'my-class'
      },
      {
        name: 'wednesday',
        required: true,
        label: 'Среда',
        align: 'center',
        field: 'wednesday',
        sortable: true,
        classes: 'my-class'
      },
      {
        name: 'thursday',
        required: true,
        label: 'Четверг',
        align: 'center',
        field: 'thursday',
        sortable: true,
        classes: 'my-class'
      },
      {
        name: 'friday',
        required: true,
        label: 'Пятница',
        align: 'center',
        field: 'friday',
        sortable: true,
        classes: 'my-class'
      }
    ],
    tableData: [
      {
        time: '10.10-11.45',
        wednesday: 'Мобильные ВС (3-1)'
      },
      {
        time: '12.05-13.40',
        wednesday: 'Мобильные ВС (3-1)',
        thursday: 'Прогр. обеспечение МС (3-23)'
      },
      {
        time: '14.10-15.45',
        tuesday: 'Прогр. обеспечение МС (4-28)',
        wednesday: 'Мобильные ВС (3-1)',
        thursday: 'Социология управления (4-3)',
        friday: 'Сборка и тест. ПП для МС (3-29)'
      },
      {
        time: '15.55-17.30',
        thursday: 'Програм. МК для МЭС (3-23)',
        friday: 'Сборка и тест. ПП для МС (3-29)'
      },
      {
        time: '17.40-19.15',
        tuesday: 'Безопасность в КС (3-29)'
      }
    ]
  })
}
</script>
