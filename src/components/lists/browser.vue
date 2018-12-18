<template>
  <div>
    <search></search>
    <tablelist :cols="cols"></tablelist>
  </div>
</template>

<script>
import search from './components/search.vue'
import tablelist from './tablelist.vue'

export default {
  name: 'browser',
  props: ['cols'],
  components: {
    search: search,
    tablelist: tablelist
  }
}
</script>

<style scoped>

</style>
