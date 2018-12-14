<template>
  <div id="app">
    <Notebook @change-page="changePage" @new-page="newPage" :pages="pages" :activePage="index" />
    <Page @save-page="savePage" @delete-page="deletePage" :page="pages[index]" />
  </div>

</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
