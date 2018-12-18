<template>
  <div>
    <textInput :enabled="true"></textInput>
  </div>
</template>

<script>
import textInput from './../../base/components/textInput.vue'

export default {
  name: 'search',
  components: {
    textInput: textInput
  }
}
</script>

<style scoped>

</style>
