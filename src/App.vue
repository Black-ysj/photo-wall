<template>
  <div id="app">
    <PhotoWall />
  </div>
</template>

<script>
import PhotoWall from './components/PhotoWall.vue'

export default {
  name: 'App',
  components: {
    PhotoWall
  }
}
</script>

<style>
  *{
    margin: 0;
    padding: 0;
  }
</style>
