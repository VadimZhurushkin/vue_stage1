<template>
  <div>
    <listItem></listItem>
  </div>
</template>

<script>
import Item from './components/listItem.vue'

export default {
  name: 'list',
  components: {
    listItem: Item
  },
  data () {
    return {
      items: []
    }
  }
}
</script>

<style scoped>

</style>
