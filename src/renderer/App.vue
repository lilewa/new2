<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
  export default {
    name: 'new2',
      mounted(){
          this.$electron.ipcRenderer.on('message', function(event, text) {
              console.log(text);

          })
      }
  }
</script>

<style>
  /* CSS */
</style>
