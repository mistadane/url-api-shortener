<template>
  <div id="app">
    <Header />
    
  </div>
</template>

<script>
import Header from './components/Header.vue'


export default {
  name: 'App',
  components: {
    Header,
    
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@500;700&display=swap');

body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: 'Poppins', sans-serif;
  font-size: 18px
}
</style>
