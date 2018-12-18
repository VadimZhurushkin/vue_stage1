<template>
  <table border="1px solid">
    <thead v-if="cols.length">
    <TableListItem :key="items[0].id" :cols="cols" :type="'head'"></TableListItem>
    </thead>
    <tbody>
    <TableListItem v-for="item in items" :cols="cols" :key="item.id" :item="item"></TableListItem>
    </tbody>
  </table>
</template>

<script>
import tableListItem from './components/tableListItem.vue'

export default {
  name: 'tablelist',
  components: {
    TableListItem: tableListItem
  },
  props: ['cols'],
  data () {
    return {
      items: [{
        id: '1',
        name: 'Иван',
        lastName: 'Петров',
        phone: '89504444422'
      },
      {
        id: '2',
        name: 'Вася',
        lastName: 'Пупкин',
        phone: '89502486552'
      },
      {
        id: '3',
        name: 'Петя',
        lastName: 'Муркин',
        phone: '89501233212'
      },
      {
        id: '4',
        name: 'Какой-то',
        lastName: 'Тип',
        phone: '88005553535'
      }
      ]
    }
  }
}
</script>

<style scoped>
  table {
    width: 100%;
    border-collapse: collapse;
  }
</style>
