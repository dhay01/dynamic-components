<template>
  <select v-model="componentName">
    <option value="Home">home</option>
    <option value="About">about</option>

  </select>
<!--this acts as a placeholder for the rendered component when toggling, we need to bind it -->
  <keep-alive>
    <component :is="componentName"></component>
  </keep-alive>

</template>
<script>
import Home from "./components/Home.vue"
import About from "./components/About.vue"

export default {
  name: "App",
  components: {
    Home, About
  },
  data() {
    return {
      componentName: "Home",
    }
  }
};

</script>