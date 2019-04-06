<template>
  <div id="app">
    <Navbar/>
    <div class="container">
      <router-view/>
    </div>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
export default {
  name: "app",
  components: {
    Navbar
  }
};
</script>

<style>
* {
  font-family: "Questrial", sans-serif;
  border-radius: 0px !important;
}
body {
  background: #f7f1f1;
}
</style>
