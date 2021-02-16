<template>
  <div id="app">
    <Title />
  </div>
</template>

<script>
import Title from "./Title";

export default {
  name: "App",
  components: {
    Title,
  },
  data() {
    return {
      hello: "Hello World",
    };
  },
  beforeCreate() {
    console.log("before created");
    console.log(this.hello);
  },
  created() {
    console.log(" created app");
  },
  beforeMount(){
    console.log("before mount")
  }
};
</script> 

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
