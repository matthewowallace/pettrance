<template>
  <div id="app">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Body/>
    <canvas class="js-canvas"></canvas>
  </div>
</template>

<script>
import HelloWorld from './components/Home.vue'
import Body from "./components/Body";
// import Nav from "./components/Nav";//

export default {
  name: 'App',
  components: {
    HelloWorld,
    Body

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
  margin-top: 0px;

}

  html, body{
    background-color: white;
    padding: 0;
    margin: 0;
  }

html {
  --scrollbarBG: #CFD8DC;
  --thumbBG: #90A4AE;
}
body::-webkit-scrollbar {
  width: 3px;
}
body::-webkit-scrollbar:hover{
  width: 10px;
}
body {
  scrollbar-width: thin;
  scrollbar-color: var(--thumbBG) var(--scrollbarBG);
}
body::-webkit-scrollbar-track {
  background: var(--scrollbarBG);
  background-color: #fff;
}
body::-webkit-scrollbar-thumb {
  background-color: var(--thumbBG) ;
  background-color: rgba(50,0,0,0.7);
  border-radius: 15px;
  border: 0px solid var(--scrollbarBG);
}
canvas{
  position: absolute;
  top: 0;
  left: 0;
  padding: 0;
  margin: 0;
  z-index: 3;
  pointer-events: none;
  mix-blend-mode: difference;
}
</style>
