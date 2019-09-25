<template lang="pug">
  li.band
    h2: a(:href="artist.url" target="_blank")  {{ artist.name }}
    img(:src="artist.image[2]['#text']")
</template>

<script>
export default {
  name: 'band',
  props: ['artist']
}
</script>

<style lang="stylus" scoped>
  li.band
    display block
    margin 10px 0
</style>
