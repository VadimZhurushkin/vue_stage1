<template>
  <div>
    <div v-if="icon"></div>
    <div v-if="caption" v-text="caption"></div>
  </div>
</template>

<script>
export default {
  name: 'pr-button',
  props: ['caption', 'icon'],
  data () {
    return {
      text: ''
    }
  }
}
</script>

<style scoped>

</style>
