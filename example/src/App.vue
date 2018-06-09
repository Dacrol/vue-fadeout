<template>
  <div id="app">
    <fadeout text="This text will be truncated because it is longer than 60 characters." :truncate-chars="60" :offset="2" :fade-chars="25" :fade="true" :dots="false"/>
    <br />
    <fadeout text="This text won't." :truncate-chars="60"/>
  </div>
</template>

<script>
import Fadeout from "vue-fadeout";

export default {
  name: "app",
  components: {
    Fadeout
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
