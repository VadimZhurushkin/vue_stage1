<template>
  <img @src="source" @alt="alt" @title="imageTitle"/>
</template>

<script>
export default {
  name: 'photo',
  props: ['source', 'alt', 'imageTitle']
}
</script>

<style scoped>

</style>
