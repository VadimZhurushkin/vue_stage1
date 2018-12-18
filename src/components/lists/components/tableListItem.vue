<template>
  <tr>
    <td v-for="colItem in cols" :key="item.id + colItem.key">
      <toggleButton v-if="type === 'head'"></toggleButton>
      {{(type === 'head' ? colItem.title : item[colItem.key])}}
    </td>
  </tr>
</template>

<script>
import toggleButton from './../../base/components/togglebutton.vue'

export default {
  name: 'tableListItem',
  components: {
    toggleButton: toggleButton
  },
  props: ['item', 'cols', 'type']
}
</script>

<style scoped>

</style>
