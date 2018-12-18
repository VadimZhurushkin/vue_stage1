<template>
  <pr-button :caption="caption" :icon="icon"></pr-button>
</template>

<script>
import button from './button.vue'

export default {
  name: 'togglebutton',
  components: {
    'pr-button': button
  },
  props: ['caption', 'icon'],
  data () {
    return {}
  }
}
</script>

<style scoped>

</style>
