<template>
  <div id="app">
    <h1>Yassin Eldeep's <span>Very Hard</span> Challenge</h1>
    <div>
      <button @click="num++">+</button>
      <p>{{ num }}</p>
      <button @click="num > 0 ? num-- : num">-</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      num: 0
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

h1 span {
  color: red;
  font-weight: bolder;
  font-size: 50px;
}

p {
  font-size: 35px;
  font-weight: bold;
}

button {
  background-color: #2c3e50;
  color: #FFF;
  text-align: center;
  border: none;
  border-radius: 20px;
  font-size: 20px;
  width: 50px;
  height: 40px;
  display: table-cell;
  vertical-align: middle;
}

button:hover {
  background-color: dimgrey;
}

</style>
