<template>
  <div id="app">
    <magnifier :options="magnifierOptions"></magnifier>
  </div>
</template>

<script>
  import magnifier from './magnifier'

  export default {
    components: {
      magnifier
    },
    data() {
      return {
        magnifierOptions: {
          width: 200,
          height: 200,
          borderSize: 2,
          borderColor: '#666666',
          shape: '',
          src: '../src/back.png',
          srcLarge: '../src/back.png'
        }
      }
    }
  }
</script>

<style scoped lang="scss">
  #app {
    margin-left: 300px;
    margin-top: 120px;
    width: 303px;
    height: 531px;
  }
</style>
