<template>
  <div id="app">
    <v-app>
      <HelloWorld msg="User"/>
      <UserListing></UserListing>
    </v-app>
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
</style>
