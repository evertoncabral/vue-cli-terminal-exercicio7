<template>
  <h1>Vue.js</h1>
</template>

<script>
export default {
  name: "Title",
  data() {
    return {};
  },
   beforeCreate() {
    console.log("before created title");
    console.log(this.hello);
  },
  created() {
    console.log(" created Title");
  },
  beforeMount(){
    console.log(this.$el)
    console.log("before mount title")
  },
  mounted(){
    console.log(this.$el)
    console.log(" mount title")
  }
};
</script>