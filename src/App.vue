<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!-- <student v-bind:message="text"> </student> -->
    <student> 
      <!-- <p slot="para">I am ok</p>
      <h1 slot="header">are you fine</h1> -->
      <div slot="header">
       <h1>Student Bio</h1>
      </div>
      <div slot="info">
       <input type="text" placeholder="Enter Name">
       <input type="text" placeholder="Enter Phone Number">
      </div>
      <div slot="details">
       <button class="btn btn-primary" v-on:click="subDetails()">Submit</button>
      </div>
      <div slot="footer">
        <p>This is your data</p>
      </div>
    </student>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import student from './components/student'

export default {
  name: 'App',
  components: {
    // HelloWorld
    student
  },
  data (){
    return {
      text : "Memory Brings back memory"
    }
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
