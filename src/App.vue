<template>
  <div id="app">
    <router-view />
  </div>
</template>

<script>


export default {
  name: 'App'
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Rubik:ital,wght@0,300..900;1,300..900&display=swap')
;

#app {
  font-family: "Rubik", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

body{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-image: url('@/assets/background.jpg');
  font-family: "Roboto", sans-serif;
}
</style>
