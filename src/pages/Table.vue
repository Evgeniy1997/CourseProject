<template>
<div>
  <q-table
    title="Расписание для группы '' на 25.12.18"
    :data="tableData"
    :columns="columns"
    row-key="name"
  />
</div>
</template>

<style>
  .q-table-container {
    margin: 86px 0px 0px 20px;
    width: 920px;
  }
</style>

<script>

export default {
  name: 'Table',
  data: () => ({
    columns: [
      {
        name: 'desc',
        required: true,
        label: 'Время',
        align: 'left',
        field: 'name',
        sortable: true,
        classes: 'my-class'
      },
      {
        name: 'desc',
        required: true,
        label: 'Понедельник',
        align: 'left',
        field: 'name',
        sortable: true,
        classes: 'my-class'
      },
      {
        name: 'desc',
        required: true,
        label: 'Вторник',
        align: 'left',
        field: 'name',
        sortable: true,
        classes: 'my-class'
      },
      {
        name: 'desc',
        required: true,
        label: 'Среда',
        align: 'left',
        field: 'name',
        sortable: true,
        classes: 'my-class'
      },
      {
        name: 'desc',
        required: true,
        label: 'Четверг',
        align: 'left',
        field: 'name',
        sortable: true,
        classes: 'my-class'
      },
      {
        name: 'desc',
        required: true,
        label: 'Пятница',
        align: 'left',
        field: 'name',
        sortable: true,
        classes: 'my-class'
      },
      {
        name: 'desc',
        required: true,
        label: 'Суббота',
        align: 'left',
        field: 'name',
        sortable: true,
        classes: 'my-class'
      }
    ],
    tableData: [
      {
        name: '8.00-9.45',
        calories: 159,
        fat: 6.0,
        carbs: 24,
        protein: 4.0,
        sodium: 87,
        calcium: '14%',
        iron: '1%'
      },
      {
        name: 'Frozen Yogurt',
        calories: 159,
        fat: 6.0,
        carbs: 24,
        protein: 4.0,
        sodium: 87,
        calcium: '14%',
        iron: '1%'
      },
      {
        name: 'Frozen Yogurt',
        calories: 159,
        fat: 6.0,
        carbs: 24,
        protein: 4.0,
        sodium: 87,
        calcium: '14%',
        iron: '1%'
      }
    ]
  })
}
</script>
