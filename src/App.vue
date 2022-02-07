<template>
  {{ message }} <br />

  Add: <button @click="increase">+1</button> <br />
  Minus: <button @click="decrease">-1</button> <br />

  Add+5: <button @click="increaseFive">+5</button> <br />
  Minus-5: <button @click="decreaseFive">-5</button> <br />

  <h2>{{ counter }}</h2>

  Name: <input type="text" v-model="name" /><br />

  Address: <input type="text" v-model="address" /><br />

  Tel: <input type="text" v-model="tel" /><br />

  Email: <input type="text" v-model="email" /><br />
  <br />

  <img v-bind:src="filename" /><br />
  <img v-bind:src="img1" /><br />
  <img v-bind:src="img2" /><br />

  <hr />

  Name: {{ name }} <br />
  Address: {{ address }} <br />
  Tel: {{ tel }} <br />
  Email: {{ email }} <br />
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
      img1: "minion1.jpg",
      img2: "minion2.jpg",
      counter: 0,
    };
  },
  components: {},
  methods: {
    increase() {
      this.counter = this.counter + 1;
    },
    decrease() {
      this.counter = this.counter - 1;
    },
    increaseFive() {
      this.counter = this.counter + 5;
    },
    decreaseFive() {
      this.counter = this.counter - 5;
    },
  },
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
