<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld/>
</template>

<script>

// import Vue from 'vue'
const HelloWorld = {
  data: function() {
    return {
      message: 'Hello World'
    }
  },
  methods: {
    test() {
      console.log("test方法执行");
    }
  },
  mounted() {
    console.log("生命周期函数执行");
  },
  render: function() {
    return (
      <div>
        <h2>Hello World Test {this.message}</h2>
        <button onClick={() => this.test()}>按钮</button>
      </div>
      )
  }
}

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
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
