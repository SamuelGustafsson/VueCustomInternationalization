<template>
  <div id="app">
    <img width="60%" src="https://financer.com/app/uploads/sites/2/zmarta-logo.jpg">
    <CustomTranslationsHandler/>
  </div>
</template>

<script>
import CustomTranslationsHandler from "./components/CustomTranslationsHandler";

export default {
  name: "App",
  components: {
    CustomTranslationsHandler
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
