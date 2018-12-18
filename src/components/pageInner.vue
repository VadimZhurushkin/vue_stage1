<template>
  <div>
    <browserView :cols="browserCols"></browserView>
  </div>
</template>

<script>
import browserView from './lists/browser.vue'

export default {
  name: 'pageInner',
  components: {
    'browserView': browserView
  },
  data () {
    return {
      browserCols: [{title: 'Ид', key: 'id'}, {title: 'Имя', key: 'name'}, {title: 'Фамилия', key: 'lastName'}]
    }
  }
}
</script>

<style scoped>

</style>
