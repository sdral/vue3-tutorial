<template>


  <div>
    <router-view></router-view>

    <br />
<div class="class1">this is app vue</div>
  
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      address: "",
      tel: "",
      email: "",
      filename: "logo.png",
      image1: "apple.jpg",
      image2: "orange.jpg",
      counter: 0,
    };
  },
  components: {},
  methods: {
    
  },
};
</script>

<style>
.class1{
  background: rgb(255, 0, 0);
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
