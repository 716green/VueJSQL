<template>
  <div id="app">
    <h1 class="heading">Main Component</h1>
    <img width="50%" src="./assets/logo.png">
    <Home/>
    <MySqlConnect/>
  </div>
</template>

<script>
import Home from "./components/Home";
import MySqlConnect from "./components/MySqlConnect";

export default {
  data: function() {
    return {
      product: {
        name: "MyJSQL"
      }
    };
  },
  components: {
    Home,
    MySqlConnect
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  text-align: center;
  margin-top: 50px;
}
.heading {
  color: orange;
}
</style>
