<template>
  <div id="app">
    <HelloWorld msg="User"/>
    <UserListing></UserListing>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import UserListing from "./components/UserListing";
export default {
  name: "App",
  components: {
    HelloWorld,
    UserListing
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
