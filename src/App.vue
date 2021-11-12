<template>
  <div id="app" class="d-flex flex-column justify-content-between">
    <Navbar />
    <b-container
        v-if="$route.name !== 'Home'"
        fluid
        class="flex-grow-1"
        :class="$route.name === 'Home' ? '' : 'darkBackground'"
    >
      <router-view class="container"/>
    </b-container>
    <router-view v-else/>
    <Footer/>

  </div>
</template>

<script>
import Navbar from "./components/Navbar";
import Footer from "./components/Footer";
export default {
  name: "app",
  components: {
    Navbar,
    Footer,
  },

  // computed: {
  //   imageUrl() {
  //     return require("@/assets/images/desktop2.png");
  //   },
  // },
};
</script>


<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

</style>
