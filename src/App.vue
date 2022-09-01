<template>

  <Nav_bar />
  <div id="app">
    <router-view />
  </div>
  <Rodape />
</template>


<script>
import Nav_bar from './components/Nav_bar.vue'
import Rodape from './components/Rodape.vue'

export default {
  name: 'App',
  components: { Nav_bar, Rodape }
}
</script>
<style>
#app {
  color: white;
  font-family: 'Roboto';
  font-size: 22px;
}

html,
body {
  margin: 0px !important;
  padding: 0px !important;
}

body {
  background-color: rgb(10, 10, 10);
}
</style>
