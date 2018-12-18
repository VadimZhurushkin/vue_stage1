<template>
  <div>
    <input v-if="enabled" type="text"/>
    <pr-label v-if="!enabled" :caption="text"></pr-label>
  </div>
</template>

<script>
import label from './label.vue'

export default {
  name: 'textInput',
  props: ['enabled', 'text'],
  components: {
    'pr-label': label
  }
}
</script>

<style scoped>

</style>
