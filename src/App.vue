<template>
  <div id="app" style="width: 960px;height: 540px;">
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
          width: 300,
          height: 300,
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
    /*margin-left: 300px;*/
    /*margin-top: 120px;*/
    /*width: 303px;*/
    /*height: 531px;*/
    margin: 100px;
  }
</style>
