<template>
  <div id="app">
    <Main />
  </div>
</template>

<script>
import Main from './components/Main.vue';


export default {
  name: 'app',
  components: {
    Main,
  },
};
</script>

<style lang="scss">
@import '@/assets/main.scss';

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

body {
  background: url('./assets/background.png') no-repeat center center fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}
</style>
